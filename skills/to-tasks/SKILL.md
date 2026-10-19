---
name: to-tasks
description: Break a spec into focused, self-contained vertical-slice task files for fresh chats.
---

Use `spec.md`, the cleaned ticket summary, and relevant codebase findings to create local implementation tasks. Flag material conflicts or missing decisions; do not guess or mark affected work Ready.

Create one focused, independently verifiable behavior per task across only the layers needed. Do not split by technical layer alone or force multiple tasks when one is sufficient. A task should have one clear outcome, bounded changes, and a focused verification path suitable for a fresh chat. Add prerequisite refactoring only when necessary; use compatible expand → migrate → contract steps for broad migrations.

Save one file per task under `tasks/<NN>-<slug>.md`, with stable IDs and blockers ordered first. Include:
- Outcome and source references.
- Acceptance criteria mapped to spec AC IDs.
- Relevant decisions, constraints, and verified code entry points.
- Dependencies and out-of-scope boundaries.
- Verification steps.
- Status: Ready, Blocked, or Needs clarification.

Each task must contain enough relevant context to start without reading the full conversation or every task. Reference specific spec sections for additional detail. Never present recommendations as agreed decisions.

Create `tasks/index.md` listing IDs, outcomes, dependencies, and statuses. Map every in-scope spec acceptance criterion to task coverage. Check for missing behavior, dependency cycles, and unnecessary duplication. Include whole-feature integration verification in the final task or a separate task only when warranted.

Mark Ready only when requirements are sufficient and dependencies are complete. Planned dependencies remain Blocked until finished. Preserve stable IDs and completion records when revising an existing breakdown.

Use the established feature folder. If none is established, ask for it. Create missing folders. Update artifacts belonging to this feature while preserving unrelated content; do not overwrite unrelated files. Return links to saved artifacts.

Return the breakdown and any blockers. Recommend one Ready task per fresh chat. Do not publish to Jira or begin implementation.
