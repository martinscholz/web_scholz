# Repository Guidelines

## Project Structure & Module Organization

This repository is a small GitHub Pages site built with Jekyll and the `minima` theme. Top-level Markdown files are site pages: `index.md` is the homepage, while `impressum.md` and `datenschutz.md` provide legal content. Shared layout fragments live in `_includes/`, currently `header.html` and `footer.html`. Site metadata and Jekyll configuration are in `_config.yml`. Ruby dependencies are declared in `Gemfile` and locked in `Gemfile.lock`; Ruby version `3.3.6` is pinned in `.ruby-version`.

## Build, Test, and Development Commands

- `bundle install`: install the GitHub Pages/Jekyll dependency set.
- `bundle exec jekyll serve`: start the local development server at `http://127.0.0.1:4000`.
- `bundle exec jekyll build`: build the static site into `_site/` and catch Jekyll rendering errors.

Run commands from the repository root. Do not edit generated `_site/` output if it appears locally.

## Coding Style & Naming Conventions

Use Markdown with YAML front matter for pages. Keep page titles explicit, for example `title: Martin Scholz`, and use sentence-style headings in page content. Prefer concise paragraphs and simple Markdown lists. In HTML includes, follow the existing two-space indentation style and preserve Liquid whitespace controls such as `{%- ... -%}` where they keep output tidy. Use lowercase, descriptive filenames for pages and assets, matching existing German legal page names where relevant.

## Testing Guidelines

There is no dedicated automated test suite in this repository. Before submitting changes, run `bundle exec jekyll build` and manually review the affected pages with `bundle exec jekyll serve`. Check links, headings, legal page routing, and responsive navigation. For content edits, verify spelling, contact details, and German compliance text carefully.

## Commit & Pull Request Guidelines

Recent commits use short, imperative summaries such as `Update homepage headline` and `Add Gemfile and local Jekyll run instructions`. Follow that style: keep the first line concise and describe the user-visible change. Pull requests should include a brief summary, the validation performed, and screenshots when visual layout or navigation changes. Link related issues when available and call out changes to legal pages or contact information explicitly.

## Security & Configuration Tips

Do not commit secrets, private tokens, or local environment files. Keep personal contact details and legal addresses accurate across `index.md`, `impressum.md`, `_config.yml`, and the footer behavior. When changing dependencies, prefer the GitHub Pages-compatible dependency path already represented by the `github-pages` gem.
