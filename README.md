# YXY Blog

A minimal Quarto blog configured for free hosting with GitHub Pages.

The public URL is configured under `website` in `_quarto.yml`:

```yaml
website:
  site-url: https://yxy92.github.io
```

The `site-url` enables correct absolute links in the RSS feed and sitemap.

## Preview locally

Install Quarto from <https://quarto.org/docs/get-started/>, then run:

```sh
quarto preview
```

## Add a post

Create a folder such as `posts/my-new-post/` and put an `index.qmd` file inside it:

```markdown
---
title: "My New Post"
description: "A one-sentence summary."
date: "2026-08-04"
categories: [notes]
---

Write the post here.
```

## Publish with GitHub Pages

1. Open or create the `yxy92/yxy92.github.io` repository.
2. Upload or push these files to its `master` branch after preserving any existing content you want to keep.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment → Source**, select **GitHub Actions**.
5. Open the **Actions** tab and wait for **Publish Quarto website** to finish.

Every later push to `master` rebuilds and publishes the blog automatically.
