# Developer Relations Activity Patterns

Companion website for the book [Developer Relations Activity Patterns](https://link.springer.com/book/10.1007/979-8-8688-1895-0), built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme. Deployed on Netlify at [devrelpatterns.com](https://devrelpatterns.com).

## Prerequisites

- [Hugo](https://gohugo.io/installation/) v0.158.0 or later (extended edition recommended)
- [Git](https://git-scm.com/)

## Setup

```bash
git clone https://github.com/stmcallister/devrelpatterns.com.git
cd devrelpatterns.com
git submodule update --init --recursive
```

The submodule step is required to pull in the PaperMod theme. Without it, Hugo will not be able to render any pages.

## Local Development

```bash
hugo server -D
```

This starts a local server at `http://localhost:1313` with live reload. The `-D` flag includes draft content.

To build the production site:

```bash
hugo --minify
```

Output goes to the `public/` directory.

## Adding Content

### Blog Posts

```bash
hugo new blog/my-post.md
```

Frontmatter fields:

```yaml
title: "Post Title"
date: 2026-01-15
draft: false
tags: ["tag1", "tag2"]
author: "Author Name"
description: "A short summary of the post."
```

### Videos

```bash
hugo new videos/my-video.md
```

Frontmatter fields:

```yaml
title: "Talk Title"
date: 2026-01-15
draft: false
youtube_id: "VIDEO_ID_HERE"
description: "A short summary of the video."
```

The `youtube_id` is the part after `v=` in a YouTube URL (e.g., `dQw4w9WgXcQ`). Thumbnails are pulled automatically from YouTube.

### Authors

Create a new file in `content/authors/`:

```yaml
title: "Author Name"
weight: 1
draft: false
photo: "/images/authors/author-name.png"
bio: "A short biography."
links:
  - name: "Website"
    url: "https://example.com"
  - name: "LinkedIn"
    url: "https://linkedin.com/in/example"
```

The `weight` field controls display order on the Authors page. Author photos go in `static/images/authors/`.

## Project Structure

```bash
content/          # Site content (blog posts, videos, author profiles)
layouts/          # Hugo layout overrides for PaperMod theme
assets/css/       # Custom CSS (extended/custom.css)
static/           # Static assets (images, etc.)
themes/PaperMod/  # Theme (git submodule — do not edit directly)
hugo.toml         # Site configuration
netlify.toml      # Netlify build settings
```

## Deployment

The site is deployed automatically via Netlify when changes are pushed to the `main` branch.
