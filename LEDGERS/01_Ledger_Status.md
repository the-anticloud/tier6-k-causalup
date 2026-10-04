# Ledger Status

**Project:** `K_CAUSALUP`  
**Tier:** TIER_6_SECURITY_EVAL  
**Identity:** Upstream `py-why/dowhy` @ `cc23521127ba` (MIT)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `py-why/dowhy` |
| Commit | `cc23521127ba21ade40514539ae7b91db27ca54a` |
| Upstream licence | MIT |
| Licence class | permissive |
| Clone size | 25.62 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1500.0 IIU |
| Verified upstream edits | 1 |

- Blocks: **0**
- Head digest: `None`
- Chain verification: **verified**

## Independent verification

The chain is verifiable without trusting this project's tooling:

```
anticloud ledger verify
anticloud ledger export > ledger.jsonl
```

Each block carries the previous block's digest, so removing or reordering an
entry invalidates every block after it. That property is the reason the
ledger can stand in for a claim of what happened.
