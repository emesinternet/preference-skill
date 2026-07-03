# Install for Generic Agent Skills

This package follows the Agent Skills folder convention:

```text
preference/
├── SKILL.md
├── agents/
└── references/
```

To install:

1. Copy `skills/preference/` into the skills directory scanned by your agent.
2. Restart or reload the agent if it only scans skills at startup.

`references/preferences.md` is intentionally omitted from the package and should be user-local. The skill creates it automatically from `references/preferences.template.md` on first use.

The portable contract is the folder plus `SKILL.md`. Agent-specific metadata such as `agents/openai.yaml` can be ignored by agents that do not use it.
