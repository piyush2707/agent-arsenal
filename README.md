# Agent Arsenal 🧰

  <img src="agent-arsenal.png" alt="Project hero banner" width="100%">
  
  <img src="agent-arsenal1.png" alt="Project hero banner" width="100%">

**Portable, practical AI-agent skills for Claude, Cursor, Codex, and other compatible coding agents.**

Agent Arsenal is an open collection of focused skills that help AI agents do software work more carefully and consistently. Each skill includes a clear workflow, safety rules, and a useful output format.

> **Project status:** Early development. Contributions, issues, and feedback are welcome.

## Skills

| Skill | What it helps with |
| --- | --- |
| [Bug Hunter](skills/bug-hunter/SKILL.md) | Investigate bugs, identify root causes, and suggest regression tests. |
| [Code Reviewer](skills/code-reviewer/SKILL.md) | Review changes for correctness, regressions, and maintainability. |
| [Security Auditor](skills/security-auditor/SKILL.md) | Spot common security risks and recommend practical mitigations. |

## Use a skill

1. Open the skill's `SKILL.md` file.
2. Follow your AI agent's instructions for adding custom skills or project instructions.
3. Copy the skill into the location supported by your agent, or paste its contents into your agent's context.
4. Review suggested changes yourself and run relevant tests before merging.

Agent tools use different discovery paths and may have different requirements. Check your tool's current documentation before installing a skill globally.

## Design principles

- **Portable:** Prefer plain Markdown and avoid unnecessary dependencies.
- **Evidence-based:** Agents must distinguish verified facts from assumptions.
- **Safe by default:** Avoid destructive changes, secret exposure, and unrelated edits.
- **Composable:** Keep each skill focused on one job.
- **Testable:** Use checklists and examples to improve skill quality over time.

## Repository structure

```text
agent-arsenal/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── .gitignore
├── .github/
│   └── workflows/
│       └── markdown-check.yml
├── skills/
│   ├── bug-hunter/
│   │   └── SKILL.md
│   ├── code-reviewer/
│   │   └── SKILL.md
│   └── security-auditor/
│       └── SKILL.md
└── tests/
    └── skill-checklist.md
```

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing a new skill or improving an existing one. Please do not include secrets, private code, or sensitive production data in issues or examples.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
