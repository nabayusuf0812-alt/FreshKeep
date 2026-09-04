# Architecture Decision Records

An ADR captures a decision that shaped the system: the **context** it was made
in, the **choice** that was made, and the **consequences** that follow. It is a
record of a moment, not a description of the current design — that lives in
[architecture.md](../architecture.md).

The value is in the reasoning. Anyone can read the code and see *what* was
chosen; only the ADR says *why*, what else was on the table, and what was
knowingly traded away. That is also the part you cannot reconstruct honestly
months later when writing the report.

## Conventions

- One file per decision, named `NNNN-short-title.md` — a four-digit number and
  a short kebab-case title, e.g. `0002-technology-stack.md`.
- Numbers are sequential and never reused, even if an ADR is rejected.
- **Never edit the decision of an accepted ADR.** If it turns out to be wrong,
  write a new ADR that supersedes it and change the old one's status to
  `Superseded by NNNN`. The wrong turn is part of the record, and being able to
  show you noticed and corrected it is worth more than a tidy history.
  Fixing a typo or a broken link is fine; changing what was decided is not.
- **Status** is one of: `Proposed`, `Accepted`, `Rejected`, `Superseded by NNNN`.

## Index

| ADR | Title | Status |
| --- | --- | --- |
| [0001](0001-record-architecture-decisions.md) | Record architecture decisions | Accepted |
| [0002](0002-technology-stack.md) | Technology stack | Proposed |
