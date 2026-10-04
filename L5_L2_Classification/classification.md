# L5 Narrow / L2 General Classification — K_CAUSALUP
**Platform:** Anticloud | **Tier:** TIER_6_SECURITY_EVAL | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
K_CAUSALUP applies causal uplift modeling to security threat prioritization: estimating the causal effect of security controls on threat likelihood. Narrow scope: Anticloud security posture analysis — not general threat intelligence.

## L2 General
L2 General: K_CAUSALUP's causal threat analysis serves all Anticloud deployment contexts. Hospital and defense deployments both use causal uplift to prioritize security investments.

## PAX 27B Integration
PAX 27B generates threat hypotheses; K_CAUSALUP tests them causally using observational data from the AIOSS chain and api-oss-logging.

## AIOSS Audit Chain
Every causal security analysis (threat vector hash + control intervention hash + uplift estimate + confidence interval) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
NIST SP 800-53 RA-3 (risk assessment). ISO 27001 A.16.1 (incident management).
