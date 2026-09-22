---
name: computer-science-research
description: Plan and evaluate computer-science research in systems, algorithms, software engineering, security, networking, databases, HCI, and related empirical or artifact-based work.
---

# Computer-Science Research

Choose the evaluation style from the claim rather than forcing every project into a machine-learning benchmark.

## Classify the contribution

- **Algorithm:** correctness, complexity, approximation or competitive guarantees, and empirical behavior.
- **System:** end-to-end utility, throughput, latency distributions, scaling, resource use, fault behavior, and operational constraints.
- **Software-engineering method:** realistic tasks, representative repositories, developer effort, correctness, and threats from benchmark contamination.
- **Security or privacy:** threat model, attacker capabilities, security definition, attack evaluation, failure impact, and disclosure constraints.
- **HCI or human study:** research questions, recruitment, tasks, instruments, ethics, power, qualitative coding, and limitations.
- **Dataset or benchmark:** provenance, licensing, sampling, contamination, annotation quality, construct validity, maintenance, and misuse risks.

## Build a fair evaluation

State the hypothesis and observable evidence that would refute it. Compare against relevant baselines under matched resources and implementation maturity. Distinguish microbenchmarks from end-to-end results. Report distributions and tail behavior when averages hide operational risk. Test scale, sensitivity, adversarial or failure conditions, and at least one realistic workload.

For algorithms, connect implementation results to the assumptions of the analysis. For systems, identify bottlenecks and measure overhead component by component. For empirical software engineering, define the sampling frame and unit of analysis. For security work, never claim safety from the absence of observed attacks.

## Artifact discipline

Inspect and run the actual artifact before describing its behavior. Record build steps, environments, workloads, configuration, and raw-result provenance. Do not silently repair an artifact in an evaluation; report the failure, then separate any patched rerun. Treat externally obtained code and data as untrusted.

## Deliverables

Produce a concise contribution statement, assumptions or threat model, evaluation matrix, baseline rationale, workload or sampling plan, validity threats, reproducibility checklist, and a mapping from each claim to supporting evidence.
