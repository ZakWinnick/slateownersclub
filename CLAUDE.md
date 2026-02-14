# CLAUDE.md

## Overview

Slate Owners Club (SOC) website — a Hugo static site for the independent Slate vehicle community. Live at https://slateownersclub.com/

## Development Commands

```bash
# Local development server
hugo server

# Build for production
hugo --minify

# Build outputs to public/
hugo
```

## Project Structure

```
content/           # Markdown content
  _index.md        # Homepage
static/images/     # Static assets (logo, hero, favicon)
themes/soc/        # Custom theme
  layouts/
    index.html     # Homepage template
    _default/      # Default templates (baseof.html, list.html, single.html)
    partials/      # Header, footer components
  static/css/      # Theme CSS
hugo.toml          # Site configuration
```

## Configuration

Key settings in `hugo.toml`:
- Primary color: `#2B2D2F` (dark slate)
- Accent color: `#D4852F` (warm amber)
- Social: @slateownersclub (X/Twitter)
- Newsletter: Buttondown
- Events: Heylo embed
- Analytics: Tinylytics
- Not affiliated with Slate Auto

## Deployment

GitHub Actions workflow (`.github/workflows/hugo.yml`) builds and deploys to GitHub Pages on push to main.
