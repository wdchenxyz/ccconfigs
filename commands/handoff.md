---
description: Generate a comprehensive handoff document for context transfer
argument-hint: [optional: specific focus area]
allowed-tools: Read, Write
---

# Project Handoff Document Generator

## Instructions

You are creating a comprehensive handoff document to transfer context to a new session. Analyze the current project state and create a detailed handoff document.

## Document Structure

Create a file called `HANDOFF.md` under docs/ in the project root with the following sections:

### 1. Current Objective
- What problem are we solving?
- Why is this important?
- What is the end goal?

### 2. Current Issue/Challenge
- Describe the specific issue we're working on
- What symptoms or errors are we seeing?
- What have we tried so far?

### 3. Project Context
- Brief overview of the project architecture
- Key technologies and frameworks in use
- Important files and their purposes
- Recent significant changes (check git log for last 5-10 commits)

### 4. Proposed Solutions/Directions
- List all approaches we've discussed
- For each approach:
  - Brief description
  - Pros and cons
  - Current status (not started/in progress/completed/abandoned)
  - Why chosen or rejected

### 5. Current Progress
- What has been completed?
- What is in progress?
- What remains to be done?
- Current blockers or dependencies

### 6. Code Changes Summary
- Files modified in this session
- Key changes made and why
- Any temporary workarounds or TODOs

### 7. Next Steps
- Immediate next actions (prioritized)
- Specific tasks to complete
- Questions that need answering
- Decisions that need to be made

### 8. Important Context
- Coding standards or patterns to follow
- Known gotchas or edge cases
- External dependencies or constraints
- Performance or security considerations

### 9. Testing Status
- What has been tested?
- What needs testing?
- Known failing tests or issues

### 10. References
- Relevant documentation links
- Related issues or tickets
- Helpful resources or examples

## Execution Steps

1. **Read the current codebase** - Focus on recently modified files
2. **Check git history** - Run `git log --oneline -10` and `git status`
3. **Review any existing documentation** - Check for README.md, docs/, .claude.md, plan.md, etc.
4. **Analyze the conversation history** - Summarize our discussion and decisions
5. **Create the HANDOFF.md file** - Write comprehensive but concise content
6. **Verify completeness** - Ensure all sections are filled with relevant information

## Output Format

- Use clear, concise language
- Include code snippets where helpful
- Use bullet points for readability
- Highlight critical information with **bold**
- Mark urgent items with ⚠️
- Mark completed items with ✅
- Mark blocked items with 🚫

## Additional Notes

If $ARGUMENTS is provided, focus the handoff document on that specific area while still providing overall context.

After creating the document, provide a brief summary of:
- The main issue we're addressing
- Current status (percentage complete estimate)
- The most critical next step
- Any urgent blockers

---

**Remember**: The goal is to enable a fresh Claude session to pick up exactly where we left off with full context and understanding.
