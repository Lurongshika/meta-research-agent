---
name: reproducible-research
description: Make computational research reproducible by structuring repositories, environments, data provenance, experiment configurations, result lineage, tests, and artifact documentation.
---

# Reproducible Computational Research

Make every reported result traceable to inputs, code, configuration, environment, and an immutable output.

## Inspect before changing

Identify the repository conventions, entry points, environment files, datasets, existing experiment runners, and generated artifacts. Preserve the user's framework and unrelated changes. Do not commit credentials, restricted data, large generated files, or machine-specific paths.

## Establish lineage

- Pin direct dependencies and record runtime, compiler, accelerator, driver, and operating-system details that can affect results.
- Separate source data, immutable intermediates, processed data, configurations, checkpoints, logs, and publication outputs.
- Give each run a stable identifier tied to the code revision, configuration, seed, and data version.
- Save raw measurements before derived tables or plots. Make transformations deterministic or document randomness.
- Keep manuscript numbers and figures generated from checked-in code or a documented artifact pipeline.

## Verification

Provide a fast smoke path and a full reproduction path. Test data loading, split invariants, metric calculations, and representative end-to-end execution. Include assertions against leakage and malformed inputs where relevant. Re-run from a clean environment when practical and compare regenerated artifacts with expected outputs using tolerances appropriate to nondeterminism.

## Honest boundaries

Differentiate repeatability on the same setup, reproducibility on an independent setup, and replication with new data or implementation. Do not call an artifact reproducible merely because code is public. Document unavailable data, proprietary dependencies, expensive compute, nondeterminism, and expected runtime.

## Deliverables

Produce or improve environment setup, data provenance, configuration layout, run commands, validation checks, artifact-generation steps, and a concise reproduction guide. Verify commands before reporting success.
