# Radon_Complexity_Lab_Results
**Project:** `K_CAUSALUP` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 3.983695652173913}`
- **complexity_grade:** `A`
- **complexity_score:** `3.983695652173913`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_CAUSALUP\UPSTREAM\example_parallel_refutation.py - A (80.98)
E:\`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_CAUSALUP\UPSTREAM\example_parallel_refutation.py
    F 14:0 example_usage - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_CAUSALUP\UPSTREAM\test_parallel_refuters.py
    F 14:0 test_refuter_source_code - B (10)
    F 50:0 test_joblib_imports - A (4)
    F 74:0 main - A (3)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_CAUSALUP\UPSTREAM\dowhy\causal_estimator.py
    M 321:4 CausalEstimator._estimate_conditional_effects - C (12)
    F 862:0 estimate_effect - B (9)
    M 619:4 CausalEstimator._test_significance_with_bootstrap - B (9)
    M 793:4 CausalEstimator.signif_results_tostr - B (9)
    M 1101:4 CausalEstimate.__str__ - B (9)
    M 517:4 CausalEstimator.estimate_confidence_intervals - B (8)
    M 207:4 CausalEstimator._set_effect_modifiers - B (7)
    M 594:4 CausalEstimator.estimate_std_error - B (7)
    M 695:4 CausalEstimator.test_significance - B (7)
    M 453:4 CausalEstimator._estimate_confidence_intervals_with_bootstrap - B (6)
    F 839:0 _warn_if_nan_in_data - A (5)
    M 556:4 CausalEstimator._estimate_std_error_with_bootstrap - A (5)
    C 37:0 CausalEstimator - A (4)
    M 267:4 CausalEstimator.estimate_effect_naive - A (4)
    M 765:4 CausalEstimator.is_bootstrap_parameter_changed - A (4)
    M 783:4 CausalEstimator.target_units_tostr - A (4)
    M 1080:4 CausalEstimate.interpret - A (4)
    M 404:4 CausalEstimator._generate_bootstrap_estimates - A (3)
    M 738:4 CausalEstimato
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_