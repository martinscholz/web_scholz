# scholz.technology

Personal website source for `https://scholz.technology`, built with GitHub Pages and Jekyll.

## Tech Stack

- GitHub Pages
- Jekyll theme: `jekyll-theme-tactile`
- Custom styles in `assets/css/style.scss`

## Project Structure

- `_config.yml`: Site configuration (theme, title, description)
- `index.md`: Homepage content
- `assets/css/style.scss`: Theme import and style overrides
- `CNAME`: Custom domain for GitHub Pages

## Local Development

1. Install Ruby and Bundler.
2. Install Jekyll and Bundler:

```bash
gem install jekyll bundler
```

3. (Recommended) Create a `Gemfile` and pin GitHub Pages dependencies.
4. Run locally:

```bash
bundle exec jekyll serve
```

5. Open `http://localhost:4000`.

## Deployment

- Push changes to the repository branch configured for GitHub Pages.
- GitHub Pages builds the site automatically.
- Domain mapping is controlled by `CNAME`.

## Customization Notes

- Global site settings live in `_config.yml`.
- To change page content, edit `index.md`.
- To customize the look, edit `assets/css/style.scss`.

