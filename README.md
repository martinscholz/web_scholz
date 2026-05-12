# Scholz

## Run locally (GitHub Pages/Jekyll)

This site is configured for GitHub Pages with Jekyll.

### 1) Install prerequisites

- Ruby 3.x. The project pins Ruby `3.3.6` in `.ruby-version`.
- Bundler (`gem install bundler`)

On macOS, avoid the built-in Apple Ruby (`ruby 2.6.x`). With Homebrew:

```bash
brew install rbenv ruby-build
rbenv install 3.3.6
rbenv local 3.3.6
gem install bundler
```

### 2) Install dependencies

```bash
bundle install
```

### 3) Start local server

```bash
bundle exec jekyll serve --livereload
```

Open: <http://127.0.0.1:4000>

If you only want to validate the static build without starting a server:

```bash
bundle exec jekyll build
```

### Common mistake

Do **not** run `source "https://rubygems.org"` in your terminal.
That line belongs in the `Gemfile` and is already provided in this repository.
