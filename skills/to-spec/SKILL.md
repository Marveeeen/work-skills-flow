---
name: to-spec
description: Write a local implementation spec from clarified requirements, agreed decisions, and codebase findings.
---

Create a concise implementation spec from `ticket-summary.md`, agreed discussion decisions, and relevant codebase findings. Use the original Jira ticket to resolve source details when needed. Flag contradictions rather than silently choosing a requirement.

Inspect relevant project instructions, architecture, code, and testing patterns. Distinguish codebase facts, agreed decisions, technical recommendations, and unverified assumptions. Do not invent product requirements or turn recommendations into approved decisions.

Save `spec.md` containing:
- Source references and intended outcome.
- Required behavior and testable acceptance criteria, with stable IDs such as AC-01.
- Scope and exclusions.
- Relevant current behavior and proposed technical approach.
- Contracts, data changes, constraints, and failure behavior where relevant.
- Verification approach, open questions, and readiness blockers.

Include enough settled requirements to plan and implement without the full chat. Avoid copying ticket filler or exhaustive code details. Always produce the requested spec; keep it brief for simple work. Mark it Draft when material decisions or confirmation remain outstanding.

Use the established feature folder. If none is established, ask for it. Create missing folders. Update artifacts belonging to this feature while preserving unrelated content; do not overwrite unrelated files. Return links to saved artifacts.

Synthesize without another interview. Do not publish to Jira or implement.
