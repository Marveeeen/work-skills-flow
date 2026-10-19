# Jira implementation workflow

1. `$clarify-ticket`: clean the ticket and agree on requirements. Save `ticket-summary.md`.
2. `$to-spec`: ground the requirements in the codebase. Save `spec.md` with stable acceptance-criterion IDs.
3. `$to-tasks`: create vertical slices in `tasks/`, with an index and criterion coverage.
4. `$implement`: implement one Ready task per fresh chat, review it, and update status.
5. `$code-review`: use during implementation or independently to review a task or feature.

Use one feature folder, for example `notes/PROJ-123/`. Pass that folder to the first skill and reuse it throughout. Each fresh implementation chat starts with its task file and only the references it needs.

On the final task, verify the complete feature against the spec. Done tasks alone do not establish end-to-end completion. Publishing, merging, and deployment require their own authorization.
