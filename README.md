# Hany Elgala — academic website

Personal academic website built with [al-folio](https://github.com/alshedivat/al-folio) for [GitHub Pages](https://helgala.github.io/personal-website/).

The first public version is intentionally minimal. Publications, teaching details, and CV content will be added from verified source documents.

## Development

This project uses Jekyll, Ruby 3.3.5, and Node 20. Run `bundle install` and `npm ci`, then `bundle exec jekyll serve` for a local preview. Run `npm run lint:prettier` and `bundle exec jekyll build` before publishing.

GitHub Actions builds and deploys the site from the default branch to GitHub Pages. Set the repository's Pages source to **GitHub Actions**.
