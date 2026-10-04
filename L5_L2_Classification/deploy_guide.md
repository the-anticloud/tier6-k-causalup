# Deploy Guide — K_CAUSALUP
**Tier:** TIER_6_SECURITY_EVAL | **Stack:** Python 3.11, causalml 0.x, PAX 27B, api-oss-logging, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, causalml 0.15+, PAX 27B, api-oss-logging access.

## Environment
8GB RAM. CPU for causal modeling. GPU for PAX hypothesis generation.

## AIOSS Integration
```bash
aioss init --module K_CAUSALUP --output ./k_causalup.aioss
aioss append --chain ./k_causalup.aioss --payload ./output.bin --module K_CAUSALUP
aioss verify --chain ./k_causalup.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="K_CAUSALUP",
    aioss_chain="./K_CAUSALUP.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_CAUSALUP.aioss --verbose
python -m K_CAUSALUP.tests.smoke
```
