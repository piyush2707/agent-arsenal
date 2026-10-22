# Contributing to Agent Arsenal

Thanks for helping improve Agent Arsenal!

## What makes a good skill?

A good skill solves one recognizable problem, gives the agent a repeatable workflow, and describes what a useful result looks like. Keep instructions practical and avoid claiming that the agent ran commands or verified behavior unless it actually did.

## Before submitting

- Keep the skill focused on one job.
- Use clear, actionable instructions.
- Separate confirmed evidence from assumptions.
- Include safety guidance for risky or destructive actions.
- Avoid unnecessary dependencies and agent-specific assumptions.
- Check the skill against [the skill checklist](tests/skill-checklist.md).
- Do not include secrets, private code, personal data, or real production logs.

## Proposing a skill

1. Open an issue describing the problem and intended users, or submit a pull request directly.
2. Add the skill under `skills/<skill-name>/SKILL.md`.
3. Use a short, lowercase, hyphenated directory name.
4. Include a concise description and a clear workflow.
5. Update the skills table in `README.md` if adding a new skill.
6. Explain any limitations or agent-specific setup.

## Pull requests

Keep pull requests small and explain the problem, the approach, and how you checked the changes. Be respectful and constructive in reviews.
