---
name: audit-code-quality
description: Audit codebase for quality issues that break AI tools. Checks file sizes, god components, duplicated logic, naming, separation of concerns, dead code, function complexity, and hardcoded values.
---

Audit this project for code quality issues that will slow me down or break my AI tool's ability to help. Check the following, in order of severity.

1. FILE SIZE
List every file over 300 lines. For each one:
- What is it doing? Is it doing too many things?
- Could it be split into smaller, focused files?
- Files over 500 lines exceed most AI tool context windows

2. GOD COMPONENTS
Find components that handle UI rendering AND data fetching AND business logic in the same file:
- Does the component manage its own API calls, state, validation, and rendering?
- Could the data fetching be separated from the display?

3. DUPLICATED LOGIC
Search for logic that appears in multiple places:
- Similar API calls in different components
- Repeated validation rules
- Copy-pasted utility functions

4. NAMING AND STRUCTURE
Check the project organization:
- Are file and folder names consistent? (camelCase vs kebab-case vs PascalCase)
- Is there a clear structure (pages/components/hooks/utils/types)?
- Can you tell what a file does from its name and location?
- Are related files grouped together or scattered?

5. SEPARATION OF CONCERNS
Check if the codebase separates:
- UI components (what users see)
- Data access (API calls, database queries)
- Business logic (rules, validation, transformations)

6. DEAD CODE
Search for:
- Commented-out code blocks (abandoned attempts, old implementations left behind)
- Unused imports
- Functions or components that are defined but never called
- Unreachable branches (conditions that can never be true)

7. FUNCTION COMPLEXITY
Find functions with high cyclomatic complexity:
- Functions with more than 5 branches (if/else, switch cases, ternaries)
- Deeply nested logic (4+ levels of nesting: if inside if inside callback inside loop)
- Nested ternary operators or dense one-liner expressions that pack multiple conditions

8. HARDCODED VALUES
Search for magic numbers, hardcoded URLs, repeated string literals, and configuration values scattered through the code instead of defined as constants or environment variables.

For each finding, report:
- Number (1, 2, 3...)
- Severity: CRITICAL, HIGH, or OK
- File and line number
- What's wrong (one sentence)
- What could happen if you don't fix it (one sentence)
- How to fix it and what could break (one sentence each)

Sort by severity, then by how fast it could hurt you.

IMPORTANT: This is an audit only. Do NOT modify any code. Report what you find and suggest fixes, but do not apply any changes until I explicitly ask you to.
