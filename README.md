# Hany Elgala — academic website

Personal academic website built with [al-folio](https://github.com/alshedivat/al-folio) for [GitHub Pages](https://helgala.github.io/personal-website/).

The site includes research, projects, publications, teaching, people, blog updates, repositories, and a downloadable CV. The publication list in `_data/publications.json` is transcribed from the July 2026 CV and cross-linked to matching Google Scholar records. It keeps patents and a manuscript under review separate from peer-reviewed publications.

## Development

This project uses Jekyll, Ruby 3.3.5, and Node 24. Run `bundle install` and `npm ci`, then `bundle exec jekyll serve` for a local preview. Run `npm run lint:prettier` and `bundle exec jekyll build` before publishing.

GitHub Actions builds and deploys the site from `main` to GitHub Pages. The repository's Pages source is configured as **GitHub Actions**.

The local `Sources/` folder holds reference materials and is ignored by Git. Only the selected headshot and July 2026 CV were copied into public `assets/`. Update the published PDF whenever the CV changes. Edit content in `_pages/`, `_posts/`, and `_data/`; keep publication status and attribution aligned with source records.
