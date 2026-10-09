# IJAS Policy & Procedure Manual (2026–2028)

The IJAS Policy & Procedure Manual as a [Just the Docs](https://just-the-docs.com) site, built for GitHub Pages.

## Publish

1. Push this folder to a GitHub repository.
2. In `_config.yml`, set `baseurl`:
   - `"/<repo-name>"` if the site will live at `https://<user>.github.io/<repo-name>/`
   - `""` for a custom domain or a `<user>.github.io` repository
3. Repository **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, branch = `main`, folder = `/ (root)`.

## Preview locally (optional)

```sh
bundle install
bundle exec jekyll serve
```

## Editing

- Each manual section is a Markdown file. Sidebar order comes from `nav_order`; nesting comes from `parent` / `has_children`.
- Internal links use `{{ site.baseurl }}{% link path/to/page.md %}`, so a broken internal link fails the build instead of silently 404ing.
- The text is kept verbatim from the PDF manual. Official forms (manual pp. 56–62) are not reproduced here; they link to the IJAS forms site.
