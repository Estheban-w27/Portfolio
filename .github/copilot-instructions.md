<!-- .github/copilot-instructions.md: Guidance for AI coding agents working on this repository -->

# Copilot instructions — Portfolio (French)

Purpose: This repository is a simple personal portfolio composed of Markdown files and an Image folder. The agent's role is to make small, careful edits to content, add assets, or improve Markdown structure while preserving the author's French language and personal information.

- **Primary files:** [index.md](../docs/01_Profil/index.md) — main portfolio page; [Script_Portfolio.md](../docs/Script_Portfolio.md) — working draft (currently empty); [exercice_syntaxe.md](../exercice_syntaxe.md) — notes and installed-extensions list.
- **Assets:** `docs/images/` — contains images referenced by the Markdown files.

Quick rules
- Keep language and tone in French when editing existing text in `index.md` and other pages.
- Preserve existing image paths (they use the `docs/images/` directory and are referenced with relative paths). Example from repo:

  ![](../docs/images/mobile-application-avatar-web-button-menu-digital-flat-style-icon-free-vector.jpg){width=100px}

- Do not introduce a site build system or change file types (no adding JS/HTML/CSS project scaffolding) unless asked — this is a static Markdown portfolio.

Editing patterns and examples
- To add a new project section, update `index.md` directly. Follow the existing Markdown style (heading levels, ordered lists, and inline links). Example pattern:

  ```markdown
  ## Nouveau Projet

  Brève description en français.

  - Technologie: Python, Markdown
  - Démo: lien ou image dans `docs/images/`
