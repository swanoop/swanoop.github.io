# swanoop.github.io

Personal portfolio and technical Field Notes site for Swanoop Ramakrishnan.

## Structure

- `index.html` — portfolio homepage entry point
- `_layouts/home.html` — homepage layout
- `_includes/` — modular portfolio sections and animations
- `blog/index.html` — Field Notes index
- `_layouts/default.html` — shared Field Notes layout
- `_layouts/post.html` — long-form article layout
- `_posts/` — published Markdown articles
- `_drafts/article-template.md` — reusable article template
- `assets/css/part-1.css` … `part-6.css` — site styling

## Publishing a Field Note

1. Copy `_drafts/article-template.md`.
2. Save the copy in `_posts/` using `YYYY-MM-DD-title.md`.
3. Update the front matter and article content.
4. Commit to `main`.
5. GitHub Pages/Jekyll will publish the article automatically and list it under `/blog/`.

The previous site is preserved on the `backup-pre-portfolio-v21` branch.
