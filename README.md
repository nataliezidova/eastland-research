# Flower in the River - Hugo Website

## What You Have

This is a complete Hugo website built in the cloud for your Eastland Disaster research and podcast. Everything is working and ready to use!

## Site Structure

```
eastland-research/
├── content/              # Your content files (markdown)
│   ├── _index.md        # Home page
│   ├── episodes/        # Podcast episodes
│   ├── research/        # Research articles
│   └── about/           # About page
├── themes/eastland/     # Your custom theme
├── public/              # Built website (ready to deploy)
└── hugo.toml           # Configuration file
```

## What's Been Created

### Custom Theme ("Eastland")
- Clean, professional design perfect for academic/research content
- Responsive layout that works on mobile and desktop
- Built-in citation display for your sources
- Episode numbering and metadata support
- Tag system for organizing content

### Sample Content
1. **Home Page** - Welcome message with recent episodes and research
2. **Episode 1**: Martha Pfeiffer - Your great-aunt's story
3. **Episode 2**: Thomas Marin - The discovery of a missing victim
4. **Research Article**: Forensic Feedback Loop methodology
5. **About Page**: Your background and research principles

### Key Features
- Automatic navigation menu
- Date-based sorting
- Citation blocks for sources
- Tag-based organization
- Clean, accessible design

## How to Add New Content

### Create a New Podcast Episode

In your terminal (when running locally), type:
```bash
hugo new episodes/episode-name.md
```

Or manually create a file in `content/episodes/` with this format:

```markdown
---
title: "Episode Title"
date: 2025-01-07
episode_number: 3
tags: ["tag1", "tag2"]
sources:
  - "Source citation 1"
  - "Source citation 2"
---

Your episode content here. You can use markdown:
- Bullet lists
- **Bold text**
- *Italic text*
- ## Subheadings
```

### Create a New Research Article

Same process, but in `content/research/`:

```markdown
---
title: "Research Title"
date: 2025-01-07
tags: ["methodology", "archival research"]
---

Your research content here.
```

## Building the Site

From the `eastland-research` directory:

```bash
# Build the site (creates/updates the public/ folder)
hugo

# Preview the site locally (opens at http://localhost:1313)
hugo server
```

## Customization Options

### Change Site Title or Description
Edit `hugo.toml`:
```toml
title = 'Your New Title'
[params]
  description = 'Your new description'
```

### Add Menu Items
Edit the `[menu]` section in `hugo.toml`:
```toml
[[menu.main]]
  name = 'New Page'
  url = '/new-page/'
  weight = 5
```

### Modify Colors/Styling
Edit `themes/eastland/layouts/_default/baseof.html` and look for the `<style>` section.

Current colors:
- Header: #2c3e50 (dark blue)
- Accent: #3498db (bright blue)
- Background: #f8f9fa (light gray)

## Deploying Your Site

The `public/` folder contains your complete, ready-to-deploy website. You can:

1. **GitHub Pages**: Push to a GitHub repository and enable Pages
2. **Netlify**: Drag and drop the `public` folder
3. **Your own hosting**: Upload the `public` folder contents via FTP

## Next Steps

1. **Customize the content** - Replace sample episodes with your real ones
2. **Add more research articles** - Document your findings
3. **Customize the design** - Adjust colors, fonts, layout to your preference
4. **Set up deployment** - Choose a hosting option and publish

## Important Notes

- All content is in **markdown** format (.md files)
- Sources automatically display in citation blocks
- Tags create automatic archive pages
- The site is static (no database needed) and very fast
- Every page is fully sourced and attributed as per your research principles

## Questions?

- Hugo documentation: https://gohugo.io/documentation/
- The theme is custom-built, so all files are editable
- Content is separate from design (content/ vs themes/)
- You own everything - no proprietary dependencies

---

**Current Status**: ✅ Site is built and ready! 45 pages generated successfully.
