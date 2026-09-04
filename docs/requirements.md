# Requirements

Every requirement here traces back to the [project charter](project-charter.md).
If a requirement does not serve the problem statement or fall inside the
charter's scope, it does not belong in this file — and if the charter's scope
needs to change to accommodate it, change the charter first, deliberately.

**Status:** draft — not yet written.

## How to read this

- **IDs are stable.** `FR-01` means the same thing for the life of the project.
  Never renumber: when a requirement is dropped, mark it retired and leave the
  ID in place. Renumbering silently invalidates every reference to it in the
  architecture, the commit history and the report.
- **Priority uses MoSCoW** — Must, Should, Could, Won't. "Won't" means *not
  this time*, recorded so it is visibly a decision rather than an oversight.
  Be honest: if everything is a Must, nothing is prioritised.
- **Verification says how it will be proven.** An automated test, a manual
  script someone can follow, a measurement. "It works" is not verification.

## Functional requirements

What the system does.

| ID | Requirement | Priority | Verification |
| --- | --- | --- | --- |
| FR-01 | As a _\<user\>_, I can _\<action\>_ so that _\<outcome\>_. | Must | _How will you prove it?_ |
| FR-02 | | | |

## Non-functional requirements

How well it does it. These are the ones most often left until too late, which
is exactly why they are numbered here alongside the functional ones.

| ID | Requirement | Priority | Verification |
| --- | --- | --- | --- |
| NFR-01 | **Performance.** _What must feel fast, and how fast? State a number and the conditions it holds under._ | | _Measured how, on what device/connection?_ |
| NFR-02 | **Accessibility.** _Target WCAG 2.1 AA unless the brief says otherwise: keyboard operable, sufficient contrast, labelled controls, works with a screen reader._ | | _Automated checks plus a manual keyboard-only pass._ |
| NFR-03 | **Privacy.** _What is collected, why it is the minimum needed, and what the user can see or delete._ | | _Reviewed against the Data section below._ |
| NFR-04 | **Reliability / offline.** _What happens with no network, or when something fails mid-action? Does data survive a restart?_ | | _Tested by simulating the failure, not by assuming it._ |

## Data

<!--
Answer these before designing storage — the answers constrain the architecture
and the technology choice.

  - What data does the system hold?
  - Where does each piece come from — entered by the user, derived, or from a
    third party?
  - Who may read it? Just its owner, or is anything shared?
  - How long is it kept, and what happens when a user deletes their account?

Assessors commonly ask specifically about personal data: what counts as
personal here, whether you need it at all, and what protects it. The strongest
answer is usually that you never collect it in the first place.
-->

_To be written._

## Open questions

Things that must be resolved before they block work — with, where possible, a
note on who can answer and by when.

- _To be written._
