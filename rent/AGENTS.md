# Repository Guidelines

## Project Structure & Module Organization
The site is a GitHub Pages project served from the repository root. Top-level documents include `index.html` for the personal landing page, `404.html` for error handling, and `CNAME` to lock the custom domain. Self-contained microsites live in dedicated directories (for example, `bd/index.html` for the birthday event); follow this pattern for new campaigns such as the upcoming `rent/` site. Keep shared assets (images, fonts, favicons) alongside the page that references them to avoid unused global folders.

## Build, Test, and Development Commands
There is no build pipeline; static pages deploy on push to the default branch. For a quick local preview, run `python3 -m http.server 4000` from the repository root and open `http://localhost:4000`. When editing several HTML files, run `npx htmlhint index.html bd/index.html` (add new paths as you create them) to catch structural mistakes before committing.

## Coding Style & Naming Conventions
Write semantic HTML with two-space indentation and closing tags on separate lines for readability. Inline critical CSS within `<style>` blocks at the top of the document, and prefer utility classes over repeated inline `style` attributes. Name new directories with short, lowercase slugs (`rent`, `launch-2024`) and keep file names lowercase with hyphens. Optimize imagery with descriptive filenames (`team-photo-2024.jpg`) and include `alt` text. Reuse existing meta tag patterns for title, description, and viewport settings.

## Testing Guidelines
Manually verify each page in desktop and mobile viewports to confirm layout responsiveness and link accuracy. Before opening a pull request, re-run `npx htmlhint` and address any warnings. Validate embedded iframes or third-party widgets by loading them over HTTPS and ensuring they render without console errors. When adding external links, confirm they open in the intended context and are free of redirects.

## Commit & Pull Request Guidelines
Adopt short, imperative commit messages (`Add rent landing skeleton`, `Fix bd hero spacing`) so the history stays scannable; avoid single-character summaries. Each pull request should describe the motivation, list visible changes, and note any manual verification steps (e.g., “Previewed locally with `python3 -m http.server`”). Include screenshots or GIFs when altering layout or styling, and link related GitHub issues when applicable to maintain traceability.
