---
name: preference
description: Capture and apply saved software development and frontend design preferences. Use setup mode when the user asks to configure or review preferences. Use apply mode when starting or planning software projects, frontend designs, architecture, stack, database, auth, email, deployment, or workflow decisions. Use capture mode when the user states an explicit ongoing preference with language like "I always prefer", "default to", or "never use".
---

# Preference

Use this skill in one of three modes.

## Mode Selection

- **Setup mode:** Use when the user explicitly asks to configure, record, update, review, or revisit preferences.
- **Apply mode:** Use when beginning or planning a software project, frontend design, stack decision, architecture decision, or project bootstrap.
- **Capture mode:** Use when the user states an explicit ongoing software or design preference during normal work.

Do not run the setup interview during apply mode or capture mode.

## Capture Mode

Capture mode is narrow. Use it only when the user clearly frames an ongoing preference with explicit preference language, such as:

- "I always prefer..."
- "I usually want..."
- "I almost always want..."
- "Default to..."
- "Never use..."
- "I hate/prefer/avoid ... in my projects..."

Do not infer an ongoing preference from a one-off instruction, critique, correction, or project-specific requirement.

Capture examples:

- "I always want buttons slightly rounded, never fully rounded or fully square."
- "Never use pill buttons in my apps."
- "Default to sidebar navigation for admin tools."
- "I usually prefer Postgres for production web apps."

Do not capture:

- "Make this button less round."
- "This screen should use a sidebar."
- "I don't like this modal."
- "Use Postgres for this project."

1. If `references/preferences.md` does not exist, create it from `references/preferences.template.md`.
2. Identify the ongoing preference and the likely category in `references/preferences.md`.
3. Read the relevant section of `references/preferences.md` before asking to save.
4. If there is no related saved preference, ask one concise confirmation before writing: "Do you want me to save that as a preference?"
5. If a related preference already exists, tell the user what is already saved and ask whether to replace it, narrow it, add an exception, or keep the existing preference.
6. If the user confirms a save or update, edit `references/preferences.md` immediately under the correct heading. Preserve the user's wording when it carries design meaning.
7. If the user does not confirm, apply the instruction only to the current task.

Completion criterion: explicit preference language was either saved after confirmation, merged with an existing related preference without duplication, or treated as current-task guidance only.

## Apply Mode

1. If `references/preferences.md` does not exist, create it from `references/preferences.template.md`.
2. Read `references/preferences.md`.
3. Apply saved preferences as defaults for relevant project decisions.
4. State the important preferences being applied only when useful for transparency.
5. Ask the user only when:
   - no saved preference exists for a relevant decision,
   - the project context clearly conflicts with a saved preference,
   - the decision is high-impact and ambiguous,
   - the user explicitly asks to choose or revisit the preference.
6. For browser inspection, UI verification, screenshots, navigation, and local web app checks, prefer Codex's internal browser or the Browser plugin before Playwright. Use Playwright only when explicitly requested, when the Browser plugin/internal browser is unavailable, or when a Playwright-only capability is required.
7. If the user states an explicit ongoing preference during project work, switch to capture mode before editing `references/preferences.md`.

Completion criterion: project decisions reflect saved preferences, and no setup-question sequence has been started unless the user requested setup mode.

## Setup Mode

1. Read `references/questions.md`.
2. If `references/preferences.md` does not exist, create it from `references/preferences.template.md`.
3. Count the total numbered questions in `references/questions.md` and track the current question's category heading.
4. Ask one question at a time using this shape:
   - `Category: <category>`
   - `Question <current> of <total> (<remaining> left)`
   - `<question text>`
   - `Options: Explain | Examples | Skip`
5. Do not show recommended answers during setup mode.
6. If the user selects `Explain`, briefly explain what decision the question is trying to capture, then ask the same question again.
7. If the user selects `Examples`, give concise examples of when someone might choose the main options, then ask the same question again.
8. If the user selects `Skip`, save no preference for that question and immediately advance to the next numbered question. Do not repeat, summarize, explain, or re-display the skipped question.
9. Accept direct answers or "decide later".
10. After each answer, update `references/preferences.md` immediately or keep a running patch and write it before ending the session.
11. Preserve prior answers unless the user explicitly changes them.

Use the `grilling` pattern: walk down the decision tree one branch at a time; do not ask multiple questions at once.

Setup mode must never acknowledge a skip and then show the skipped question again. After `Skip`, the next assistant message should contain only the next distinct question and its setup metadata.

Completion criterion: every answered preference from the setup session is saved in `references/preferences.md`, and unanswered preferences remain visibly unset.

## Storage Format

Store preferences in `references/preferences.md` using concise headings and bullets. Each saved answer should include:

- the preference,
- any caveat or condition the user gave,
- the date if the user frames it as provisional or time-sensitive.

Use plain language. Do not over-normalize the user's wording when the wording itself is a design preference.
