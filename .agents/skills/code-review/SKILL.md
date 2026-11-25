---
name: code-review
description: Review Laravel code changes for correctness, security, maintainability, performance, business-rule compliance, and test coverage. Use when reviewing implementations, pull requests, or recently modified files.
---

# Code Review Skill

## Review Priorities

1. Correctness
2. Business-rule compliance
3. Security vulnerabilities
4. Authorization issues
5. Database integrity
6. Performance
7. Maintainability
8. Test coverage

## Review Guidelines

- Read the relevant requirements.
- Inspect the actual code changes.
- Check edge cases.
- Check unauthorized access scenarios.
- Check validation and error handling.
- Identify duplicated logic.
- Check for N+1 queries.
- Verify that tests cover important behavior.

## Output

Report findings by severity:

- Critical
- High
- Medium
- Low

For each finding, include:

- File and location
- Problem
- Impact
- Suggested solution

Do not modify files unless explicitly requested.
