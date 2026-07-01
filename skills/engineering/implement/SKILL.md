---
name: implement
description: "Implement a piece of work based on a spec or set of tickets."
disable-model-invocation: true
---

Implement the work described by the user in the spec or tickets.

If the user passes a ticket reference, fetch it from the issue tracker and state its title before starting. If the reference is ambiguous, ask.

Call the Skill tool with "tdd" where possible, at pre-agreed seams.

Run typechecking regularly, single test files regularly, and the full test suite once at the end.

Once every PRD/issue item is implemented and typechecks and tests pass, call the Skill tool with "mattpocock-skills:code-review" on the diff before committing anything. Code review runs as isolated sub-agents that only report findings back to you.

After you've addressed the findings, commit your work to the current branch.
