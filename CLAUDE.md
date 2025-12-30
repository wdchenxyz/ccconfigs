# Project Memory Guide
The project utilizes a centralized knowledge base in the `docs/` directory to maintain continuity across development sessions.

**Instruction for Claude**: Always invoke the `project-memory` skill when performing architectural changes, starting new features, or debugging.

## Documentation Index

### 📍 [Context & Overview](docs/context.md)
- **Purpose**: The "Source of Truth" for the project's current state.
- **Content**: Project vision, high-level tech stack, and a "Current Focus" section.
- **Usage**: Read this at the start of every session to understand the immediate goals.

### 🏗️ [Architecture & Standards](docs/architecture/)
- **Purpose**: Permanent technical rules and system design.
- **Content**: Data models (ERDs), API specifications, folder structures, and coding conventions.
- **Usage**: Consult these files before scaffolding new modules to ensure consistency.

### 🗺️ [Plans & Roadmap](docs/plans/)
- **Purpose**: Future-facing tasks and implementation details.
- **Content**: `backlog.md` for ideas and specific `feature-*.md` files for active development.
- **Usage**: Update these files with "Done" checkboxes as you complete sub-tasks.

### 🐞 [Issues & Lessons Learned](docs/issues/)
- **Purpose**: Historical record of problems and their solutions.
- **Content**: Root cause analysis, reproduction steps, and "Lesson Learned" for every major bug.
- **Usage**: Search this folder when encountering cryptic errors to see if they've been solved before.

### ⚖️ [Decision Log (ADR)](docs/decisions/)
- **Purpose**: Tracking the "Why" behind technical choices.
- **Content**: Architecture Decision Records (ADR) documenting trade-offs (e.g., choosing a specific library).
- **Usage**: Refer to this to avoid re-litigating past technical decisions.

---

## Developer Workflow Commands
- **New Task**: "Initialize a new plan for [Feature] in docs/plans/"
- **Debug**: "Check docs/issues/ for similar problems, then start debugging"
- **Finish**: "Generate a PR summary and update docs/context.md and the relevant plan"
