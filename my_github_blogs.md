---
description: Instructions for adding new blog posts to giulioruffini.github.io
---

# How to update the Blogs page

This site is a Jekyll + Minimal Mistakes GitHub Pages site. Blog posts are either **standalone HTML files** hosted locally in `assets/blogs/`, or **external links** to posts on BCOM Confluence, Neuroelectrics, or Substack.

## Adding a new local blog post

1. Place the standalone HTML file in `assets/blogs/` (e.g., `assets/blogs/my-new-post.html`)
2. Open `blogs.md` and add a new entry under the **"Hosted here"** section:
   ```markdown
   - [Post Title](/assets/blogs/my-new-post.html) — Short description
   ```
3. Commit and push:
   ```bash
   git add assets/blogs/my-new-post.html blogs.md
   git commit -m "Add blog: Post Title"
   git push origin recovery
   ```

## Adding a link to an external blog post

1. Open `blogs.md` and add a new entry under the appropriate section (**BCOM Foundation blog**, **Neuroelectrics blog**, or **Substack**):
   ```markdown
   - [Post Title](https://full-url-to-the-post) (Month Year)
   ```
2. Commit and push:
   ```bash
   git add blogs.md
   git commit -m "Add blog link: Post Title"
   git push origin recovery
   ```

## File reference

| File | Purpose |
|------|---------|
| `blogs.md` | The Blogs listing page (permalink: `/blogs/`) |
| `assets/blogs/` | Directory for standalone HTML blog files |
| `_data/navigation.yml` | Top navigation menu (already includes "Blogs") |
| `index.md` | Home page (already links to `/blogs/`) |

## Notes

- Local blog posts are self-contained HTML with embedded CSS — they do not use the Jekyll layout system.
- The blog listing in `blogs.md` is manually maintained — add new entries at the top of the relevant section to keep newest posts first.
- After pushing, GitHub Pages typically rebuilds within 1-2 minutes.
- The site deploys from the `recovery` branch.
