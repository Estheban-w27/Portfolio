<!-- .github/copilot-instructions.md: Guidance for AI coding agents working on this repository -->

# Copilot instructions — Portfolio (French)

Purpose: This repository is a simple personal portfolio composed of Markdown files and an Image folder. The agent's role is to make small, careful edits to content, add assets, or improve Markdown structure while preserving the author's French language and personal information.

- **Primary files:** [Index.md](Index.md) — main portfolio page; [Script_Portfolio.md](Script_Portfolio.md) — working draft (currently empty); [exercice_syntaxe.md](exercice_syntaxe.md) — notes and installed-extensions list.
- **Assets:** `Image/` — contains images referenced by the Markdown files.

Quick rules
- Keep language and tone in French when editing existing text in `Index.md` and other pages.
- Preserve existing image paths (they use the `Image/` directory and are referenced with relative paths). Example from repo:

  ![](Image/mobile-application-avatar-web-button-menu-digital-flat-style-icon-free-vector.jpg){width=100px}

- Do not introduce a site build system or change file types (no adding JS/HTML/CSS project scaffolding) unless asked — this is a static Markdown portfolio.

Editing patterns and examples
- To add a new project section, update `Index.md` directly. Follow the existing Markdown style (heading levels, ordered lists, and inline links). Example pattern:

  ```markdown
  ## Nouveau Projet

  Brève description en français.

  - Technologie: Python, Markdown
  - Démo: lien ou image dans `Image/`
  ```

- To add images: place files into `Image/` and reference them relatively (e.g., `Image/mon-image.png`). Keep filenames descriptive and avoid changing other images' names.

Workflow / developer hints (discoverable in repo)
- The repository contains VS Code-focused tooling notes in `exercice_syntaxe.md`. Recommended extensions already listed there: "French Language Pack", "Markdown All in One", "Markdown Preview Enhanced", and a French spell checker.
- Preview and edit Markdown using VS Code's Markdown Preview (`Ctrl+K V`) or the installed preview extensions.

Conventions & constraints
- Language: French for content edits.
- Minimal structural changes only: refactors of Markdown structure (headings, lists, images) are OK; do not create new build pipelines or introduce server-side code.
- Personal data: `Index.md` contains personal contact info; do not alter contact details unless explicitly instructed by the repo owner.

When to ask the user
- If a requested change implies a site build, new dependency, or conversion to a different format (e.g., static-site generator), ask for explicit approval and a target tool (e.g., Jekyll, Hugo).
- If personal/contact information needs to change, confirm exact replacement text.

Examples of safe edits
- Fix Markdown typos, improve headings, swap an image for a clearer one placed in `Image/`, or add a new project section in `Index.md`.

Examples of edits to avoid without confirmation
- Adding code or runtime dependencies, setting up CI, or converting repository into a compiled site.

If uncertain, stop and ask: produce a short diff proposal and ask the repository owner to confirm.

---
Please review these instructions and tell me if you want the agent to: (a) update content in French, (b) add new projects/images, or (c) convert the repo to a static site generator — then I will proceed.
