# Install for Claude

Copy the same portable skill folder into Claude's skills directory.

For Claude Code, a common personal install location is:

```bash
mkdir -p ~/.claude/skills
cp -R ./skills/preference ~/.claude/skills/preference
```

On Windows PowerShell:

```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.claude\skills" | Out-Null
Copy-Item -Recurse -Force .\skills\preference "$env:USERPROFILE\.claude\skills\preference"
```

`references/preferences.md` is created automatically from `references/preferences.template.md` the first time the skill needs to read or save preferences.

For project-local use, copy `skills/preference` into the project's Claude skills location if your Claude environment scans project skills.

Invoke by asking Claude to use the Preference skill, or use your client-specific skill invocation syntax.
