# Developer Cookbook — K_CAUSALUP
**Stack:** Python 3.11, causalml 0.x, PAX 27B, api-oss-logging, AIOSS_FORMAT
**Domain:** Causal uplift modeling for security threat prioritization in Anticloud

## Threat uplift analysis
```python
from k_causalup import SecurityUpliftAnalyzer

analyzer = SecurityUpliftAnalyzer(
    pax_model="./pax-27b-q4.gguf",
    log_db="./api_oss_logging.db",
    aioss_chain="./causalup.aioss"
)

result = analyzer.analyze(
    treatment="enable_mfa_for_pax_api",
    outcome="unauthorized_access_attempts",
    confounders=["time_of_day", "request_volume"]
)
print(f"ATE: {result.ate:.3f} (p={result.p_value:.4f})")
print(f"Recommendation: {result.recommendation}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
