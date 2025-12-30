---
name: project-memory
description: Manages project context and structured documentation. Use this skill when starting new tasks, debugging issues, finalizing features, or whenever the user asks for project context. This skill guides Claude to read/write structured files in the docs/ directory to maintain long-term project memory.
---

# Project Memory Skill

## Workflow

1. **Task Initialization**: Before writing code, prioritize reading `docs/context.md` and `docs/architecture/` to ensure all implementations align with established project standards and technical stacks.
2. **Issue Troubleshooting**: When a bug is reported, search `docs/issues/` for similar historical entries. After resolving the bug, create a new record documenting the root cause and prevention steps.
3. **Plan Execution**: Create or update implementation checklists within `docs/plans/` to track progress and maintain a clear roadmap for the current feature.
4. **Knowledge Loop (Closing)**: Upon task completion, generate a comprehensive PR Summary and backfill this information into the relevant documents (plans or issues) to close the context loop.

## Documentation Standards

- **Context Maintenance**: Always keep the "Current Focus" or "Progress" section in `docs/context.md` updated after every major change.
- **Decision Tracking**: Every significant technical trade-off or architectural change must be recorded as an ADR (Architecture Decision Record) in `docs/decisions/`.
- **Consistency**: Ensure that all new files and code snippets follow the naming conventions and folder structures defined in `docs/architecture/`.

## Trigger Keywords
- "What is the current status?"
- "Start a new feature/task"
- "Fix this bug"
- "Summarize my changes"
- "Update the documentation"
