# 3-Seed Simulation — K_CAUSALUP

**Seeds:** `19371` · `50708` · `84907`

**Seed method:** `sha256("K_CAUSALUP")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_CAUSALUP`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.2663 | 0.0146 | ±0.0286 |
| throughput_tokens_per_sec | 1078.3667 | 25.7858 | ±50.5402 |
| p50_latency_ms | 44.52 | 4.6103 | ±9.0362 |
| p99_latency_ms | 110.4467 | 1.5085 | ±2.9567 |
| ttft_ms | 25.73 | 1.4142 | ±2.7718 |
| mmlu_proxy | 0.714 | 0.0 | ±0.0 |
| hellaswag_proxy | 0.7937 | 0.0168 | ±0.0329 |
| truthfulqa_proxy | 0.5643 | 0.0514 | ±0.1007 |
| arc_proxy | 0.7305 | 0.0159 | ±0.0312 |
| complexity_cyclomatic | 3.3233 | 0.0377 | ±0.0739 |
| maintainability_index | 77.7233 | 4.3511 | ±8.5282 |
| security_issues_high | 0.0 | 0.0 | ±0.0 |
| dependency_freshness_pct | 80.4333 | 6.8825 | ±13.4897 |
| test_coverage_pct | 49.1333 | 0.2357 | ±0.462 |
| doc_coverage_pct | 62.5333 | 2.3099 | ±4.5274 |
| memory_mb | 204.7333 | 6.7411 | ±13.2126 |
| gpu_util_pct | 65.0333 | 6.6939 | ±13.12 |
| openssf_score | 7.0 | 0.3394 | ±0.6652 |
| eu_ai_act_compliance_pct | 84.9 | 6.5054 | ±12.7506 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 19371 | Seed 50708 | Seed 84907 |
|--------|------------|------------|------------|
| trl_score | 7.256 | 7.287 | 7.256 |
| throughput_tokens_per_sec | 1096.6 | 1041.9 | 1096.6 |
| p50_latency_ms | 47.78 | 38.0 | 47.78 |
| p99_latency_ms | 109.38 | 112.58 | 109.38 |
| ttft_ms | 24.73 | 27.73 | 24.73 |
| mmlu_proxy | 0.714 | 0.7139 | 0.714 |
| hellaswag_proxy | 0.8056 | 0.7699 | 0.8056 |
| truthfulqa_proxy | 0.5279 | 0.637 | 0.5279 |
| arc_proxy | 0.7418 | 0.708 | 0.7418 |
| complexity_cyclomatic | 3.35 | 3.27 | 3.35 |
| maintainability_index | 80.8 | 71.57 | 80.8 |
| security_issues_high | 0 | 0 | 0 |
| dependency_freshness_pct | 85.3 | 70.7 | 85.3 |
| test_coverage_pct | 49.3 | 48.8 | 49.3 |
| doc_coverage_pct | 60.9 | 65.8 | 60.9 |
| memory_mb | 209.5 | 195.2 | 209.5 |
| gpu_util_pct | 60.3 | 74.5 | 60.3 |
| openssf_score | 7.24 | 6.52 | 7.24 |
| eu_ai_act_compliance_pct | 89.5 | 75.7 | 89.5 |
| slsa_level | 1 | 2 | 1 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._