# Technical Research Agent for Codex

This plugin began as a Codex-native adaptation of the skill architecture from
[matheus-rech/meta-agent](https://github.com/matheus-rech/meta-agent) and has
been redesigned for machine learning, computer science, and mathematics.

## Included skills

- Machine-learning experimental design and audit
- Computer-science research evaluation
- Mathematical proof development and checking
- Technical literature reviews with citation verification
- Reproducible computational research artifacts
- Technical paper drafting and claim-to-evidence review

## Compatibility and safety

The upstream Claude Agent SDK orchestration layer is intentionally excluded.
These skills run under Codex and use only tools available in the active Codex
session. They must not claim to have searched a database, inspected an
artifact, executed an experiment, or proved a theorem unless the relevant work
was actually performed. Unexecuted code and computational evidence are labeled
clearly.

## Attribution

The MIT license is preserved in `LICENSE`. The current domain instructions are
an independent Codex-focused redesign and do not imply endorsement by the
upstream author.
