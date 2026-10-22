# Skill Quality Checklist

Use this checklist when creating or reviewing a skill in Agent Arsenal.

## Metadata and purpose

- [ ] The file is named `SKILL.md`.
- [ ] YAML frontmatter contains a clear `name` and `description`.
- [ ] The name matches the skill's directory and uses lowercase hyphenated words.
- [ ] The description says what the skill does and when to use it.
- [ ] The skill focuses on one recognizable task.

## Instructions

- [ ] Steps are actionable, ordered, and easy to follow.
- [ ] The skill says what evidence or context the agent should inspect.
- [ ] It distinguishes confirmed facts from assumptions.
- [ ] It defines a useful final report or output.
- [ ] It avoids unsupported claims about tools, tests, or results.

## Safety and reliability

- [ ] Risky or destructive actions require appropriate confirmation.
- [ ] Secrets and sensitive data are protected.
- [ ] The instructions discourage unrelated changes.
- [ ] The skill does not encourage bypassing tests or security controls.
- [ ] Limitations and unresolved questions are reported honestly.

## Portability and maintenance

- [ ] Instructions are primarily plain Markdown.
- [ ] Agent-specific assumptions are documented.
- [ ] Examples are generic and contain no private or production data.
- [ ] README documentation is updated if the skill is added or renamed.
