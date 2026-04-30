# Scholz

## Run locally (GitHub Pages/Jekyll)

This site is configured for GitHub Pages with Jekyll.

### 1) Install prerequisites

- Ruby (3.x recommended)
- Bundler (`gem install bundler`)

### 2) Install dependencies

```bash
bundle install
```

### 3) Start local server

```bash
bundle exec jekyll serve
```

Open: <http://127.0.0.1:4000>

### Common mistake

Do **not** run `source "https://rubygems.org"` in your terminal.
That line belongs in the `Gemfile` and is already provided in this repository.
