---
name: mathematical-reasoning
description: Develop, check, and explain mathematical definitions, conjectures, proofs, counterexamples, symbolic derivations, and computational experiments across pure and applied mathematics.
---

# Mathematical Reasoning

Prioritize correctness, explicit assumptions, and traceable logical dependencies.

## Establish the statement

- Normalize notation and quantify every variable.
- State domains, regularity conditions, boundary cases, and whether objects may be empty, infinite, singular, random, or degenerate.
- Separate definitions, assumptions, lemmas, theorem statements, and consequences.
- Before proving a claim, test small, extreme, and adversarial cases; search for a counterexample when the statement looks too strong.

## Construct the argument

Choose a proof strategy that matches the structure: direct proof, contrapositive, contradiction, induction, extremal argument, invariant, compactness, probabilistic method, reduction, or explicit construction. Track where each assumption is used. Do not hide the critical step behind phrases such as “clearly” or “standard” when it carries the result.

Check algebra, signs, dimensions, convergence, interchange of limits/integrals/expectations, and equality cases. For asymptotics, state which variables tend where and what constants may depend on. For probability, identify the probability space, conditioning, independence, and almost-sure versus in-expectation claims.

## Computational support

Use symbolic or numerical computation to explore, falsify, or verify bounded instances—not as a substitute for proof unless the theorem is explicitly computer-assisted. Preserve exact arithmetic when floating-point error could change the conclusion. Record software, precision, bounds, and verification scope. Never describe sampled evidence as a universal proof.

## Review mode

When checking a proof, locate the first unsupported inference, give a counterexample if possible, classify the gap as local or structural, and propose the smallest valid repair. Distinguish a correct proof with exposition problems from an incorrect theorem.

## Deliverables

Return a precise statement, proof idea, complete derivation at the requested level, assumption ledger, boundary-case check, and—when useful—an independent verification or counterexample search.
