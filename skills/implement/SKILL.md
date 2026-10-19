---
name: implement
description: Implement one ready task, verify acceptance criteria, and update task status.
---

Implement the selected local task. State its title and read its requirements, dependencies, referenced spec sections, and applicable project instructions. Load additional context only as needed.

Verify dependencies are complete. Stop dependent work when blocked. Investigate factual uncertainty through code and documentation; ask about unresolved consequential decisions instead of changing requirements.

Record the starting change scope so review can distinguish this task from pre-existing work. Follow project branch rules, architecture, and testing patterns. Preserve unrelated changes. Deliver all task acceptance criteria without unrelated refactoring or adjacent tasks.

Use TDD where appropriate and available. Run relevant tests, typechecking, and required project checks. Run broader tests when required or justified by the change. Record failed or unavailable checks honestly.

Review the task diff using `code-review` when available; otherwise review correctness, regressions, standards, and requirement coverage directly. Fix actionable issues introduced by the task and rerun affected checks.

Update the task and index status and record concise verification results and remaining issues. Use In progress while working, Blocked when progress requires an unmet prerequisite, and Done only when acceptance criteria and required checks pass. Refresh dependent task readiness.

When the final task finishes, verify the complete feature against the spec acceptance criteria, including integration checks. Report any remaining gaps; completed individual tasks alone do not establish feature completion.

Return changes, verification, current status, and the next Ready task. Do not automatically begin another task unless the user authorized the sequence. Commit only when requested or already authorized. Do not publish, merge, or deploy unless authorized.
