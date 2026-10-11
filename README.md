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

On Linux, install Ruby build dependencies first. For Debian/Ubuntu:

```bash
sudo apt update
sudo apt install -y git curl build-essential libssl-dev libreadline-dev zlib1g-dev
```

Then install Ruby `3.3.6` with your preferred version manager. With `rbenv`:

```bash
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init - bash)"' >> ~/.bashrc
source ~/.bashrc
rbenv install 3.3.6
rbenv local 3.3.6
gem install bundler
```

### 2) Install dependencies

```bash
bundle install
```

### 3) Test the build

```bash
bundle exec jekyll build
```

This generates the static site in `_site/` and verifies that Jekyll can render the pages.

### 4) Start local server

```bash
bundle exec jekyll serve
```

Open: <http://127.0.0.1:4000>

### Common mistake

Do **not** run `source "https://rubygems.org"` in your terminal.
That line belongs in the `Gemfile` and is already provided in this repository.
