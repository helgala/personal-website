# Hany Elgala — academic website

Personal academic website built from the [Academic Pages](https://academicpages.github.io/) template and its [Minimal Mistakes](https://michaelrose.dev/minimal-mistakes/) runtime for [GitHub Pages](https://helgala.github.io/personal-website/).

The site includes research, publications, teaching, software, posts, and a downloadable CV. Publications are rendered as Academic Pages collection entries and link to the owner’s Google Scholar records. Source documents remain private in the local `Sources/` directory; only the selected headshot and CV are published.

## Development

This project uses Jekyll and GitHub Pages. Run `bundle install` and `npm ci`, then `bundle exec jekyll serve` for a local preview. Run `npm run lint:prettier` and `bundle exec jekyll build` before publishing.

GitHub Actions builds and deploys the site from `main` to GitHub Pages. The repository’s Pages source is configured as **GitHub Actions**. The reference framework files live in `_layouts`, `_includes`, `_sass`, `assets/css`, `assets/js`, and `images`; site-specific content lives in `_pages`, `_publications`, `_research`, and `_posts`.

## Content workflow

- Edit the main pages in `_pages`. Add or remove top-level navigation items in `_data/navigation.yml`.
- Add publications as one Markdown file per item in `_publications`, research areas in `_research`, and news or articles in `_posts`.
- Store public PDFs in `assets/pdf` and link to them from the relevant page. Keep private source documents in `Sources/`; that directory is excluded from the generated site.
- Preview changes locally with `bundle exec jekyll serve`, then check the layout at a narrow mobile width as well as on a desktop screen before pushing.
- Push reviewed changes to `main`. GitHub Actions runs the formatting check, builds the Jekyll site, and deploys the result to GitHub Pages.

The current project URL is `https://helgala.github.io/personal-website/`. A future move to the shorter `helgala.github.io` address or a custom domain would require a separate repository or domain configuration change.
