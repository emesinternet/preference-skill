# Preference Skill

Preference is a portable Agent Skill for capturing and applying saved software development and frontend design preferences.

## Why This Exists

AI coding agents are more useful when they remember how you like to build. Without that context, every new project starts with the same repeated choices: which database to use, how the frontend should be structured, what kind of navigation feels right, how much testing is expected, where content should live, and how polished the first version should be.

This skill turns those recurring decisions into a reusable preference file. You answer the setup questions once, then the agent can apply those defaults later without interviewing you again. It can also capture new ongoing preferences when you state them clearly during normal work.

The goal is not to lock every project into one rigid stack. It is to give the agent a practical starting point, reduce repeated clarification, and make early product, engineering, and design decisions feel more like working with someone who already knows your taste.

It supports three workflows:

- **Setup mode:** walk through preference questions one at a time.
- **Apply mode:** silently apply saved preferences when planning or building projects.
- **Capture mode:** detect explicit ongoing preference language during normal work, confirm with the user, then save the preference.

Setup mode is not required. It is a good starting point for most fullstack developers because it builds a useful baseline before project work begins. The setup questionnaire is 173 questions long. Each setup question shows its category, progress, and remaining question count. It does not show recommendations by default; users can ask for `Explain`, `Examples`, or `Skip`.

The skill follows the open Agent Skills folder format: a `SKILL.md` file with YAML frontmatter plus optional `references/` and agent-specific metadata.

## Package Contents

```text
skills/preference/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── preferences.template.md
    └── questions.md
```

`references/preferences.md` is intentionally not included. The skill creates it from `preferences.template.md` automatically on first use.

## Install

- Codex: see [install/codex.md](install/codex.md)
- Claude: see [install/claude.md](install/claude.md)
- Generic Agent Skills: see [install/generic.md](install/generic.md)

## Usage Examples

Setup:

```text
Use $preference to configure my project preferences.
```

Apply:

```text
Build a SaaS dashboard and apply my saved preferences.
```

Capture:

```text
I always want buttons slightly rounded, never fully rounded or fully square.
```

The skill should ask before saving a captured preference.

## License

MIT
