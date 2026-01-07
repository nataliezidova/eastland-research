# Quick Start Guide

## Most Common Tasks

### 1. Add a New Podcast Episode

Create a new file: `content/episodes/new-episode.md`

```markdown
---
title: "Episode Title Here"
date: 2025-01-07
episode_number: 5
tags: ["relevant", "tags"]
sources:
  - "Source 1"
  - "Source 2"
---

Episode content goes here...
```

### 2. Preview Your Changes

```bash
cd eastland-research
hugo server
```

Open browser to: http://localhost:1313

### 3. Build for Publishing

```bash
cd eastland-research
hugo
```

Your site is now in the `public/` folder, ready to upload anywhere.

### 4. Update the About Page

Edit: `content/about/_index.md`

### 5. Change Site Settings

Edit: `hugo.toml` (site title, menu, etc.)

## File Locations Cheat Sheet

- **Content**: `content/` folder
  - Episodes: `content/episodes/`
  - Research: `content/research/`
  - About: `content/about/`
  
- **Design/Theme**: `themes/eastland/layouts/`
  - Base template: `baseof.html`
  - Home page: `home.html`
  - Episode/article pages: `single.html`
  - Archive pages: `list.html`

- **Built Site**: `public/` folder (upload this to web host)

- **Configuration**: `hugo.toml` (root folder)

## Markdown Syntax Reminders

```markdown
# Heading 1
## Heading 2
### Heading 3

**bold text**
*italic text*

- Bullet point
- Another point

1. Numbered list
2. Second item

[Link text](https://example.com)

> Quote block
```

## Tips

- Front matter (between `---` lines) is metadata
- Everything after front matter is your content
- Hugo rebuilds automatically when you save files (in server mode)
- Tags automatically create archive pages
- Sources display in a special citation block on each page

## Workflow

1. Write/edit content in markdown files
2. Run `hugo server` to preview
3. Make changes, save, refresh browser
4. When happy, run `hugo` to build
5. Upload `public/` folder to hosting

That's it!
