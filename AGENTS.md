# Repository Guidelines

## Project Structure & Module Organization
- Root files: `README.md` (authoritative list), `index.md` (site mirror), `_config.yml` (Jekyll), `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `LICENSE`.
- Add or edit resources in `README.md`. Mirror essential changes to `index.md` when needed for the website.

## Build, Test, and Development Commands
- GitHub Pages: pushing to the default branch publishes automatically.
- Local preview (no Gemfile provided):
  - Install Ruby, then: `gem install jekyll jekyll-feed jekyll-theme-cayman`.
  - Serve with live reload: `jekyll serve --livereload` (visit http://localhost:4000).
  - Build static site: `jekyll build` (outputs to `_site/`).

## Coding Style & Naming Conventions
- Markdown only. Use `#`/`##` headings; bullets start with `-`.
- Entries: `[Title](URL) — one‑sentence description` (concise, factual). Optional level tag: `(Beginner|Intermediate|Advanced)`.
- Order links alphabetically within sections unless a clear thematic order exists.
- Keep headings in Title Case; anchors in kebab‑case. Wrap lines ~100 chars.

## Testing Guidelines
- No unit tests. Validate that `jekyll build`/`serve` completes without errors.
- Manually verify: links resolve, no duplicates, section anchors work, and front matter remains intact in `index.md`.

## Commit & Pull Request Guidelines
- Commits: imperative, concise, scoped. Suggested prefixes: `docs:`, `content:`, `site:`.
  - Example: `content: add TextAttack to Tools`.
- PRs must include: brief description, rationale, section updated, and (if UI-visible) a screenshot of the rendered block.
- Ensure compliance with `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md`. One topic per PR.

## Agent-Specific Notes
- Prefer minimal edits limited to `README.md`, `index.md`, and `_config.yml` (when changing site settings).
- Do not modify `LICENSE` or `CODE_OF_CONDUCT.md` unless explicitly requested.
- Avoid adding new build dependencies or assets. Preserve existing formatting and section order.
- When in doubt, open an issue proposing the change before large edits.

