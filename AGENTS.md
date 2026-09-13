# Academic website project

This is Hany Elgala's personal academic website. It uses the al-folio Jekyll starter and publishes to GitHub Pages from `main`.

## Content and sources

- Use the owner's supplied CV, publications, existing site, and other documents as the basis for biographical and academic claims.
- Preserve exact names, titles, dates, affiliations, authorship, and links from their sources. Flag conflicts or missing details rather than inventing them.
- Distinguish published work from work in progress or under review when the sources do.
- Keep source documents separate from public website assets unless the owner chooses to publish them.

## Development workflow

- Keep site-specific content in `_pages`, `_data`, `_bibliography`, and `assets`. Runtime styling and layouts come from al-folio plugin gems unless a documented local override is needed.
- Make changes in small, reviewable steps. Use Git branches or Codex worktrees once this directory has a repository.
- Check the site's layout on narrow and wide screens. Run `npm run lint:prettier` and `bundle exec jekyll build` where Ruby 3.3.5 and Bundler are available; verify the GitHub Actions build before publishing.
- Keep credentials out of tracked files. Use the GitHub sign-in or credential flow instead of placing tokens in project files.
