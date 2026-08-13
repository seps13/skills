---
name: implement
description: "Implement a piece of work based on a spec or set of tickets."
disable-model-invocation: true
---

Implement the work described by the user in the spec or tickets.

Use /tdd where possible, at pre-agreed seams.

Run typechecking regularly, single test files regularly, and the full test suite once at the end.

Once every PRD/issue item is implemented and typechecks and tests pass, invoke /mattpocock-skills:code-review on the diff before committing anything. Code review runs as isolated sub-agents that only report findings back to you — they must not commit, push, or re-invoke /implement or any review skill themselves.

After you've addressed the findings, commit your work to the current branch.
