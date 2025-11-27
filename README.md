# Hana X AI

Personal portfolio and projects site built with Jekyll and hosted on GitHub Pages.

## Live Site

**https://hana-x-ai.github.io**

## Structure

```
├── index.md              # Homepage
├── about.md              # About page
├── projects.md           # Projects listing
├── articles.md           # Articles/blog listing
├── _layouts/             # Page templates
├── _posts/               # Blog articles (YYYY-MM-DD-title.md)
├── _projects/            # Project entries
└── assets/css/           # Styling
```

## Adding Content

### New Article
Create a file in `_posts/` with format `YYYY-MM-DD-title.md`:

```markdown
---
layout: post
title: "Your Article Title"
date: 2025-11-26
tags:
  - tag1
  - tag2
---

Your content here...
```

### New Project
Create a file in `_projects/`:

```markdown
---
title: Project Name
description: Short description
tags:
  - tag1
github: https://github.com/...
---

Project details here...
```

## Local Development

```bash
# Install dependencies
bundle install

# Run locally
bundle exec jekyll serve

# View at http://localhost:4000
```

## Tech Stack

- **Jekyll** - Static site generator
- **GitHub Pages** - Hosting
- **Kramdown** - Markdown processor
- **Custom CSS** - Dark theme styling

## License

MIT
