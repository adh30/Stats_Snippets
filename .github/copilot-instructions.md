<!-- .github/copilot-instructions.md - Guidance for AI coding agents -->
# Copilot instructions for this repository

Purpose: Help AI coding agents be immediately productive in the `Stats_Snippets` repository.

Key points (quick):
- **Repo type:** A small collection of statistical documentation/snippets (Markdown). See `README.md`.
- **Primary file patterns:** single-file Markdown snippets at repo root, e.g. `logged_variables_in_regression.md`.
- **No build/test system:** There is no code, build, or CI in this repository—produce and edit content, not binaries.

Big picture
- This repository is a curated set of standalone statistical notes and derivations. Each file is meant to be readable and self-contained. Agents should treat changes as documentation edits, not software changes.
- Typical workflow: author drafts a short Markdown file containing an explanation, derivation, and minimal metadata (author/version/date).

Project-specific conventions
- File location: place new snippets at the repository root, using descriptive lowercase underscores, e.g. `my_new_snippet.md`.
- Metadata header: keep (when present) the `Author`, `Version`, and `Date` fields at the top of the file like `logged_variables_in_regression.md`.
- Math: use LaTeX inline `$...$` and display `$$...$$` or fenced math as shown in `logged_variables_in_regression.md`. Maintain existing formatting.
- Tone and length: concise, explanatory, and aimed at a statistically-literate reader (e.g., clinicians, economists). Keep examples brief and focused.
- Citations & claims: do not invent references or data. If adding a claim that requires citation, flag it and ask the user for the correct source.

Editing guidance (concrete)
- Preserve the document header lines `**Author:**`, `**Version:**`, `**Date:**` when updating content unless the user requests metadata edits.
- When reformatting math or Markdown, keep line breaks and paragraphs readable (wrap ~80 chars where reasonable).
- If converting verbal derivations to numbered steps, follow the existing style: short numbered steps with inline math (see `logged_variables_in_regression.md` for example).
- Avoid adding executable code blocks unless the user explicitly asks to include an example script; this repo is documentation-first.

Pull request / commit guidance
- Commit message template: `docs: add|update <short-file-name.md> - <one-line description>`
- PR title template: `Docs: <short description> — add/update snippet`.
- Explain changes in the PR description: what was clarified, what math or notation changed, and whether metadata (`Author`, `Version`, `Date`) were updated.

When to ask the user (be explicit)
- If a claim needs an external citation, stop and ask for the source.
- If you plan to add new file metadata (new author or version scheme), ask before changing conventions.
- If converting a text derivation into code or reproducible analysis, propose creating a separate code example and ask for permission.

Examples from this repo (use as templates)
- `logged_variables_in_regression.md` — short author/version/date header, LaTeX math, numbered derivation steps, practical interpretation section.
- `README.md` — single-line repo description. Keep README minimal when adding new snippets; add a short index entry only if the user asks.

Don'ts
- Don't fabricate experiments, datasets, or citations.
- Don't add test/build configs or pretend a CI exists.

If unclear or incomplete: ask a single clarifying question rather than making assumptions.

End of instructions.
