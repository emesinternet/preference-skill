# Install for Codex

Copy the skill folder into your Codex skills directory:

```powershell
Copy-Item -Recurse -Force .\skills\preference "$env:USERPROFILE\.codex\skills\preference"
```

On macOS/Linux:

```bash
mkdir -p ~/.codex/skills
cp -R ./skills/preference ~/.codex/skills/preference
```

`references/preferences.md` is created automatically from `references/preferences.template.md` the first time the skill needs to read or save preferences.

Invoke explicitly with:

```text
Use $preference to configure my project preferences.
```

Codex can also invoke the skill implicitly when its description matches the current work.
