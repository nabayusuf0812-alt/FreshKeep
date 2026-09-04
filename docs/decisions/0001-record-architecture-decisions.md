# 0001 — Record architecture decisions

- **Status:** Accepted
- **Date:** 2026-09-04

## Context

A capstone project is assessed partly on engineering judgement, not only on
whether the finished thing runs. Early decisions — how the project is
structured, what it depends on, where the interfaces sit, how data is shaped —
constrain everything built afterwards, and they are made when the least is
known.

Left unrecorded, the reasoning does not survive. Reconstructing it months later
while writing the report produces rationalisation: a tidy justification for
whatever happened to be built, written by someone who already knows how it
turned out. That is much weaker evidence of judgement than a record written
before the outcome was known — including the decisions that later proved wrong.

## Decision

Record each architecturally significant decision as a numbered Markdown file in
`docs/decisions/`, committed alongside the code it affects.

**Significant** means expensive to reverse: project structure, dependencies and
frameworks, interfaces between components, and how data is modelled or stored.
Routine choices — a variable name, a helper function, how one screen is laid
out — need no ADR.

Write the ADR when the decision is taken, not afterwards.

## Consequences

- The rationale for each significant choice is captured while it is still
  fresh, and is directly quotable in the final report.
- There is a small, recurring writing cost per decision. Keeping ADRs short
  keeps that cost honest — a page is plenty.
- The git history shows when each decision was taken relative to the code,
  which is itself evidence that the reasoning came first rather than after.
