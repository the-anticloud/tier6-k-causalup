# HF_Leaderboard_Lab_Results

**Project:** `K_CAUSALUP`  
**Tier:** `TIER_6_SECURITY_EVAL`  
**Slug:** `py-why/dowhy`  
**Commit:** `cc23521127ba`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **43.34 ms** |
| Min latency | 37.0 ms |
| Max latency | 48.49 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **35** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5878 |
| Classification latency | 70.48 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_CAUSALUP (py-why/dowhy) — 528 files, 53037 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'causal', '##up', '(', 'p', '##y', '-', 'why', '/', 'dow', '##hy', ')', '—', '52', '##8', 'files', ',', '530']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_