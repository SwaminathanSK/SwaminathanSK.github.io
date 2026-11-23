# swaminathansk.github.io

Personal site and blog, built by GitHub Pages with Jekyll. Pushing to `master` deploys it.

## Writing a blog post

Add a Markdown file to `_posts/` named `YYYY-MM-DD-short-title.md`:

```markdown
---
title: "My post title"
description: "One line shown under the title on the blog list (optional)."
math: true   # optional: renders $inline$ and $$display$$ LaTeX
---

Write the post here in Markdown.

![Caption](/assets/posts/my-figure.png)
```

- The post's URL becomes `/blog/YYYY/short-title/`.
- Put images for posts in `assets/posts/`.
- To keep a post unpublished, add `published: false` to its front matter.
- Posts are listed only on the Blog page (not on the home page).

## Adding a paper or project

Edit `_data/publications.yml` or `_data/projects.yml` and copy an existing entry. Put the thumbnail in `data/`.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | About page (bio, research interests, papers) |
| `research/index.html` | Publications and projects, generated from `_data/` |
| `blog/index.html` | List of all posts |
| `_layouts/`, `_includes/` | Shared page shell, top navigation, post layout |
| `assets/style.css` | Styles |
| `data/` | Photos and paper thumbnails |

## Previewing locally (optional)

```bash
sudo apt install ruby-dev build-essential
gem install --user-install jekyll -v '~> 3.10' jekyll-feed jekyll-seo-tag kramdown-parser-gfm webrick
jekyll serve   # then open http://localhost:4000
```
