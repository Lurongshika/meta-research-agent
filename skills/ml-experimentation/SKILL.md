---
name: ml-experimentation
description: Design, implement, audit, and interpret machine-learning experiments, including datasets, baselines, ablations, metrics, leakage checks, uncertainty, and reproducibility.
---

# Machine-Learning Experimentation

Turn a research question into evidence that distinguishes real model improvement from leakage, tuning luck, or an unfair comparison.

## Frame the claim

- State the task, population or data-generating process, inputs, outputs, constraints, and intended generalization target.
- Identify the exact claim: predictive improvement, efficiency, robustness, calibration, interpretability, or a causal effect. Do not substitute one for another.
- Choose the simplest credible baseline and at least one competitive reference method. Match preprocessing, data access, tuning budget, and evaluation protocol.

## Protect the evaluation

- Split by the unit that can leak information: subject, user, device, document family, time, site, or graph component—not merely rows.
- Fit preprocessing, feature selection, augmentation policies, threshold selection, and hyperparameter search on training data only.
- Preserve a final test set when repeated iteration would otherwise tune to it. For small data, use nested cross-validation or repeated resampling where appropriate.
- Record seeds, versions, dataset identifiers, split manifests, hardware, precision, and stopping rules.

## Measure what matters

- Select metrics from the decision context and class balance. Report more than accuracy for imbalanced tasks.
- Include uncertainty: confidence intervals, variation across seeds or folds, and paired comparisons when runs share examples.
- Separate statistical detectability from practical importance. Report effect sizes and resource cost.
- Use ablations that isolate the proposed contribution. Change one interpretable factor at a time unless interactions are the question.
- Check distribution shift, subgroups, calibration, failure cases, and compute/memory/latency when relevant.

## Execution discipline

Inspect the repository, data schema, and existing evaluation code before modifying anything. Reuse the project framework unless the user requests a new one. Run inexpensive smoke tests before full experiments. Never present unexecuted code, incomplete runs, or invented metrics as results. If compute or data is unavailable, deliver an executable protocol and label expected outcomes as hypotheses.

## Deliverables

Provide the experimental question, data and split policy, baselines, model variants, tuning budget, metrics, uncertainty method, ablations, stopping rule, reproducibility details, and a results table whose rows map directly to runnable configurations.
