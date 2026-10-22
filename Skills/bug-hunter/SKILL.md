---
name: bug-hunter
description: Investigate software bugs, trace likely root causes, propose minimal fixes, and identify regression tests. Use when debugging errors, unexpected behavior, or failing tests.
---

# Bug Hunter

## Goal

Find the most likely cause of a reported software bug and recommend the smallest safe correction supported by available evidence.

## Workflow

1. **Clarify the failure.** Identify the observed behavior, expected behavior, reproduction steps, and relevant error messages.
2. **Inspect context.** Review the relevant source, tests, configuration, recent changes, and logs that are available.
3. **Reproduce when possible.** Run a minimal reproduction or the most relevant test if tools and environment permit. Never claim a reproduction succeeded unless it did.
4. **Trace the cause.** Follow the failing data or control flow. Distinguish confirmed facts from hypotheses and rank hypotheses by evidence.
5. **Choose a minimal fix.** Preserve existing architecture and conventions; avoid unrelated refactors.
6. **Check side effects.** Consider edge cases, compatibility, error handling, and callers affected by the change.
7. **Add regression coverage.** Suggest or implement a focused test that would fail before the fix and pass after it, where appropriate.
8. **Verify honestly.** Run relevant checks when available and report the exact commands and results. If unable to run them, say so.

## Safety rules

- Do not modify unrelated files.
- Do not delete tests or weaken assertions just to make a check pass.
- Do not expose credentials, tokens, or sensitive data found in logs.
- Ask before destructive actions or changes with significant external impact.
- If evidence is insufficient, state what is missing instead of inventing a root cause.

## Final report

Provide:

- **Cause:** confirmed root cause or best-supported hypothesis.
- **Evidence:** files, functions, logs, or tests that support the conclusion.
- **Fix:** proposed or completed changes.
- **Tests:** commands run and their actual results.
- **Risks:** remaining uncertainty or follow-up work.
