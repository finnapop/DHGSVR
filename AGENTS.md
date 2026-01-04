# Repository Guidelines

## Project Structure & Module Organization
This repository is a static site. HTML pages live at the repo root: `index.html`,
`index_v1.html`, `2026.html`, and `code.html`. Images and other assets also sit at
the root (`avatar.png`, `2026.jpeg`). GitHub Pages deployment is configured in
`.github/workflows/static.yml` and publishes the entire repository.

## Build, Test, and Development Commands
No build step or package manager is used.
- Local preview (simple web server): `python3 -m http.server`, then open
  `http://localhost:8000/index.html`.
- Quick file preview: open an HTML file directly in a browser if you do not need
  relative asset paths tested.

## Coding Style & Naming Conventions
Use 2-space indentation in HTML and CSS. Styles are embedded in each HTML file
inside a `<style>` block with CSS variables declared under `:root`. Class names
are BEM-like (`nav__brand`, `hero__text`) with modifiers such as
`.button.secondary`. Keep file names short and descriptive; new pages should live
in the repo root.

## Testing Guidelines
There are no automated tests. Manually verify:
- Page loads without console errors.
- Images resolve from root-relative paths.
- Responsive layout works at mobile and desktop widths.

## Commit & Pull Request Guidelines
Recent commits are short and action-oriented (for example, "Update index.html" or
"Create 2026.html") with occasional Japanese; follow the same concise style and
mention the primary file or feature. For pull requests, include a brief summary,
note any new assets, and add before/after screenshots for visual changes. Ensure
the GitHub Pages workflow remains green.
