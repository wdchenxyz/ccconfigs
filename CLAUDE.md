---

## Developer Workflow Commands
- **New Task**: "Initialize a new plan for [Feature] in docs/plans/"
- **Debug**: "Check docs/issues/ for similar problems, then start debugging"
- **Finish**: "Generate a PR summary and update docs/context.md and the relevant plan"

## Research Mode
- Before starting any task, deeply research the codebase to understand architecture, coding style, and tech stacks.

## Plan Mode
- Make the plan extremely concise. Sacrifice grammar for the sake of concision.
- At the end of each plan, give me a list of unresolved questions to answer, if any.

## Project Memory Guide
The project utilizes a centralized knowledge base in the `docs/` directory to maintain continuity across development sessions.

**Instruction for Claude**: Always invoke the `project-memory` skill when performing architectural changes, starting new features, or debugging. If there are not initialized documents in the `docs/` folder, create them as per the structure below.
