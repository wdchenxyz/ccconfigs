## Post-Mortem Analysis Protocol

After successfully resolving a difficult or lengthy troubleshooting session, automatically initiate a post-mortem by:

### 1. Session Summary
- **Problem Statement**: Concise description of the original issue
- **Duration/Complexity**: Note if the session was particularly challenging
- **Final Solution**: What ultimately resolved the issue

### 2. Critical Analysis
- **What Went Wrong**: Identify missteps, incorrect assumptions, or inefficient approaches
- **What Went Right**: Highlight effective strategies and breakthrough moments
- **Missed Signals**: Early clues that were overlooked or misinterpreted
- **Time Sinks**: Steps that consumed disproportionate effort without progress

### 3. Root Cause Analysis
- **Surface Issue vs. Root Cause**: Distinguish between symptoms and underlying problems
- **Why It Was Hard**: What made this problem particularly challenging?
- **Knowledge Gaps**: What information would have accelerated the solution?

### 4. Generalizable Learnings
Extract principles that apply beyond this specific case:
- **Pattern Recognition**: "Problems of type X often manifest as Y"
- **Diagnostic Heuristics**: "When you see A and B together, check C first"
- **Anti-Patterns**: "Avoid doing X when troubleshooting Y"
- **Tool/Technique Recommendations**: Specific commands, logs, or methods that proved valuable

### 5. Troubleshooting Guide Entry
Create a reusable guide entry with:
- **Title**: Descriptive name for this problem class
- **Symptoms**: How to recognize this issue
- **Common Causes**: Ranked by likelihood
- **Diagnostic Steps**: Ordered checklist for investigation
- **Solutions**: Proven fixes with context for when to apply each
- **Prevention**: How to avoid this issue in the future
- **Related Issues**: Links to similar problem patterns


### 6. Persist the Knowledge
1. **Generate a markdown file** with the following naming convention:
   - `troubleshooting-guide-[problem-domain]-[YYYY-MM-DD].md`
   - Example: `troubleshooting-guide-docker-networking-2024-03-15.md`

2. **Provide the complete file content** in a code block for the user to save

3. **Instruct the user** to save this file in their troubleshooting knowledge base directory

4. **For future sessions**, prompt the user:
   - "Do you have any troubleshooting guides from previous sessions? Please share relevant ones."
   - "I can reference guides from past sessions if you upload them to this conversation."

5. **Maintain an index file** (`troubleshooting-index.md`) that lists all guides with:
   - Problem domain
   - Date created
   - Key symptoms/tags
   - Filename reference
