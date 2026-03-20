# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Companion website for the book "Developer Relations Activity Patterns" — a Hugo static site using the PaperMod theme, deployed on Netlify.

## Development Commands

```bash
# Local development server
hugo server -D          # -D includes draft content

# Build for production
hugo --minify

# Create new content
hugo new blog/my-post.md
hugo new videos/my-video.md
hugo new authors/author-name.md
```

Hugo version: 0.158.0 (specified in `netlify.toml`).

## Architecture

- **Theme**: PaperMod, installed as a git submodule in `themes/PaperMod`. Do not edit theme files directly — use layout overrides instead.
- **Layout overrides** in `layouts/`: custom partials for Giscus comments (`partials/comments.html`), homepage with book cover (`partials/home_info.html`), and custom list pages for `authors/` and `videos/` sections.
- **Custom CSS**: `assets/css/extended/custom.css` — PaperMod's extension point for styles.
- **Comments**: Giscus (GitHub Discussions-based), configured in `hugo.toml` under `[params.giscus]`.

## Content Sections

Content lives in `content/` with three sections:
- **blog/**: Standard posts with `title`, `date`, `tags`, `author`, `description` frontmatter.
- **videos/**: YouTube video entries using `youtube_id` in frontmatter; thumbnails are auto-generated from YouTube.
- **authors/**: Author profiles with `photo`, `bio`, `weight` (for ordering), and `links` (array of `{name, url}`) in frontmatter.

## Deployment

Netlify auto-deploys from the main branch. Build command: `hugo --minify`, publish directory: `public/`.
