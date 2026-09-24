# Personal Webpage

Source for [ferdinand-popp.github.io](https://ferdinand-popp.github.io/).

Built with [Jekyll](https://jekyllrb.com/), using only plugins whitelisted by
GitHub Pages (`jekyll-feed`, `jekyll-seo-tag`, `jekyll-sitemap`), so it builds
automatically on push — no CI step required.

## Structure

- `_config.yml` — site settings (title, author, social links)
- `_data/publications.yml` — publication list (shown on `/publications/`)
- `_data/cv.yml` — CV content (shown on `/cv/`)
- `_data/teaching.yml` — talks, posters, and teaching (shown on `/teaching/`)
- `_posts/` — news items (shown on the homepage). Projects live entirely on
  GitHub — the nav and homepage link straight there instead of a local page.
- `_blog/` — longer-form posts (shown on `/blog/`); create the folder and add
  `YYYY-MM-DD-slug.md` files with `title:` front matter the same way as `_posts/`
- `_layouts/`, `_includes/` — page templates
- `assets/css/style.css` — theme

## Local preview

Requires Ruby + Bundler:

```
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## Editing content

- New publication → add an entry to `_data/publications.yml`
- New news item → add a Markdown file to `_posts/` named `YYYY-MM-DD-slug.md`
  with `title:` front matter
- New blog post → same, but in `_blog/`
- CV changes → edit `_data/cv.yml`
- Teaching/talks changes → edit `_data/teaching.yml`

## Credits

Icons by [Font Awesome](https://fontawesome.com/). Code released under a
[Creative Commons Attribution-ShareAlike 3.0 International License](http://creativecommons.org/licenses/by/3.0/).
