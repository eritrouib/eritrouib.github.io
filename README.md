# @ET: data, maps and decisions

Personal website and blog of Eriola Trungu Impersimi, built with [Quarto](https://quarto.org) and hosted on GitHub Pages.

## Write and preview

1. Install Quarto: <https://quarto.org/docs/get-started/> (one-time).
2. In this folder:
   ```
   quarto preview
   ```
   A browser opens and refreshes as you edit.

## Add a post

1. Copy a folder in `posts/`, e.g. `posts/2026-11-my-new-post/`, and edit its `index.qmd`.
2. Update the `title`, `description`, `date` and `categories` at the top.
3. Put images in the same folder and use `![Caption](image.png)`.
4. Add `draft: true` at the top while you're still writing; remove it to publish.

Posts can contain live Python or R code blocks; Quarto runs them when it builds the site.

## Publish

```
quarto render
git add .
git commit -m "New post"
git push
```

`quarto render` writes the finished site to `docs/`. GitHub Pages serves it (Settings → Pages → Deploy from a branch → main, /docs).

## Where things are

| File | What it is |
|---|---|
| `_quarto.yml` | Site settings: title, menu, links |
| `styles.scss` | Colours and fonts (the @ET palette) |
| `index.qmd` | Home page |
| `blog.qmd` | Blog listing |
| `projects.qmd` | Projects page |
| `about.qmd` | About page |
| `posts/` | One folder per post |
| `assets/et-mark.svg` | The @ET logo and favicon |
