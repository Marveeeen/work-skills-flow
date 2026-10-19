# Personal Jira-to-Implementation Skills

These skills are customized for my development workflow and inspired by [Matt Pocock’s skills](https://github.com/mattpocock/skills). They are adapted versions for my needs, rather than an official or unchanged copy of that collection.

## My workflow

Start with a Jira ticket, remove unnecessary wording without losing requirements, and establish shared understanding before implementation. Turn that understanding into a codebase-grounded spec, then split the work into focused vertical slices suitable for fresh chats.

| Step | Skill            | Purpose                                                                                        | Output                          |
| ---- | ---------------- | ---------------------------------------------------------------------------------------------- | ------------------------------- |
| 1    | `clarify-ticket` | Summarize Jira, ask focused questions, challenge assumptions, and confirm shared understanding | `ticket-summary.md`             |
| 2    | `to-spec`        | Combine clarified requirements, agreed decisions, and codebase findings                        | `spec.md`                       |
| 3    | `to-tasks`       | Create self-contained vertical slices with acceptance criteria and dependencies                | `tasks/index.md` and task files |
| 4    | `implement`      | Implement one ready task, verify it, review changes, and update progress                       | Code changes and task status    |
| 5    | `code-review`    | Check requirement coverage, correctness, regressions, and project standards                    | Actionable review findings      |

`code-review` supports implementation and can also be used independently.

## How I use them

Use one feature folder, such as `notes/PROJ-123/`, throughout the workflow. Provide the ticket and folder to `clarify-ticket`, then pass the saved artifacts to subsequent steps.

Start each implementation task in a fresh chat with its task file. Read only the referenced spec sections and code needed for that task. Keep task dependencies and statuses current. When the final task finishes, verify the complete feature against the spec rather than relying only on individual task completion.

## Behaviors preserved

- Ask questions in rounds and settle prerequisite decisions before dependent ones.
- Synthesize agreed context into a spec without restarting the interview.
- Split work by verifiable behavior, rather than technical layer.
- Implement, test, and review against acceptance criteria.
- Review both requirement alignment and code quality.

## Personal adaptations

- Jira supplies the original requirements; agreed changes are recorded explicitly.
- Local Markdown artifacts carry decisions between chats.
- Questions focus on material gaps rather than exhaustive interrogation.
- Tasks stay bounded without unnecessary splitting.
- Publishing to Jira, committing, merging, and deploying are not automatic.
