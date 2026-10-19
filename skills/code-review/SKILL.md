---
name: code-review
description: Review task changes for correctness, regressions, standards, and requirement coverage.
---

Review selected task changes without modifying code unless fixes are requested or already authorized.

Use the supplied diff, PR, or comparison reference; otherwise use the task's recorded starting scope. Account for relevant committed, staged, unstaged, and untracked changes without duplicate reporting or attributing unrelated work to this task. Verify the comparison; ask if its scope cannot be established reliably. Use merge-base comparisons for branch changes and exact comparisons when requested.

Read the task, relevant spec sections, agreed clarifications, and applicable project standards. Consult the ticket summary or Jira for missing source details when available. Flag requirement conflicts and missing review context.

Review through two lenses:
- Requirements: missing acceptance criteria, incorrect behavior, and unintended scope changes.
- Code quality: bugs, regressions, security, data integrity, meaningful test gaps, and documented standards.

Inspect surrounding code and tests. Focus on actionable issues introduced by the changes. Code smells are investigative hints, not automatic findings. Avoid preference-only suggestions or unrelated refactoring. Use focused checks to verify suspected issues when useful.

Independent reviewers may be used when available and useful. Verify and deduplicate their findings before reporting.

List findings by severity, labeling each Requirements or Code quality. Include file and line when applicable, triggering condition, impact, supporting evidence, and a concise correction. Distinguish verified findings from uncertainty. Separate optional suggestions from blockers.

State checks performed and limitations. If no actionable findings remain, say so without implying complete assurance. Do not mark tasks Done based on review alone or commit, publish, or expand scope without authorization.
