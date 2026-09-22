# Meta Research Agent for Codex

This is a Codex-native port of the domain skills from
[matheus-rech/meta-agent](https://github.com/matheus-rech/meta-agent).

## Included skills

- Neurosurgery literature-search strategy
- Structured study-data extraction
- Risk-of-bias assessment
- Conventional meta-analysis planning and interpretation
- Network meta-analysis
- Trial sequential analysis
- PRISMA-compliant manuscript drafting

## Compatibility and safety

The upstream Claude Agent SDK orchestration layer is intentionally excluded.
These skills run under Codex and use only tools available in the active Codex
session. They must not claim to have searched a database, read a paper, or run
an analysis unless the relevant source or execution tool was actually used.

R-dependent analyses require a working local R installation and the referenced
packages. When R is unavailable, the plugin can design, review, and explain the
analysis but must clearly label code and numerical results as unexecuted.

## Attribution

Original project copyright and license are preserved in `LICENSE`. Adaptation
adds Codex plugin metadata and compatibility instructions; it does not imply
endorsement by the upstream author.
