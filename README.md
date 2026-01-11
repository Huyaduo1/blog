# BlogWeb

Minimal Hugo-based personal site with a resume-style homepage and a blog list.

## Tech Stack

- Hugo (static site generator)
- Custom templates in `layouts/`
- Custom styles in `assets/css/custom.css`

## Project Structure

- `content/` content pages and posts
- `layouts/` Hugo templates
- `assets/` CSS and other assets processed by Hugo Pipes
- `res/` static assets (images, etc.)

## Local Development

```bash
hugo server -D
```

Then open the URL printed in the terminal.

## Deployment

This repo is configured for GitHub Pages via GitHub Actions.
Push to `main` and the site will be built and deployed automatically.

## Notes

- If you change the GitHub Pages path, update `baseURL` in `hugo.toml`.
- Static files are served from both `static/` and `res/`.
