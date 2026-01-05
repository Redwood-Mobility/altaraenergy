# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Altara Energy website - a Jekyll-based static site for an EV charging network. Hosted on GitHub Pages at altaraenergy.com.

**Brand positioning**: Standalone EV charging brand, part of Pathfinder Rewards loyalty network. Operated by Rangeway (not prominently customer-facing). Focus on convenience, not premium/luxury.

**IMPORTANT**: Do NOT use "city EV charging" or "city charging" as a descriptor. Altara is simply an EV charging network - no geographic qualifier needed.

## Build & Development Commands

```bash
# Install dependencies
bundle install

# Local development server
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

The site builds automatically on GitHub Pages when pushed to main branch.

## Project Structure

```
/
├── _config.yml          # Jekyll config, site metadata, SEO settings
├── _layouts/default.html # Base HTML template
├── _includes/
│   ├── header.html      # Nav, meta tags, structured data
│   └── footer.html      # Footer with links, social icons
├── assets/css/style.css # All styles (includes dark mode)
├── images/              # Logo variants (SVG files)
└── index.html           # Homepage (currently the main page)
```

Root-level reference materials (not part of build):
- `ALTARA_WEBSITE_PROJECT_BRIEF.md` - Full brand positioning and content guidelines
- `altara-brand-guidelines-v2.html` - Visual brand guidelines
- `Logo/` - Original logo source files

## Key Configuration

**_config.yml** contains:
- Site metadata and SEO settings
- Social media links (@altaraenergy handles)
- Build exclusions for reference materials

**Gemfile**: Uses `github-pages` gem for GitHub Pages compatibility.

## Brand Guidelines

- **Colors**: Current Teal (#0891B2), Ember Orange (#F97316), Deep Teal (#0E7490)
- **Typography**: Outfit font via Google Fonts
- **Logo files**: Located in `images/` (altara-logo-standard.svg, altara-logo-white.svg, altara-logo-mono-teal.svg, plus icon variants)
- **Language**: NEVER use "city EV charging" or "city charging". Avoid premium/luxury positioning.
- **Social handles**: @altaraenergy (Twitter/X, Instagram), altara-energy (LinkedIn)

## Content Guidelines

- **NEVER use "city EV charging" or "city charging"** - Altara is simply an EV charging network
- Focus on convenience, efficiency, accessibility
- Pathfinder Rewards is the loyalty program (multi-network)
- Avoid premium/luxury/adventure language
- See `ALTARA_WEBSITE_PROJECT_BRIEF.md` for full messaging guidelines

## Dependencies

- Jekyll (via github-pages gem)
- jekyll-seo-tag plugin
- Font Awesome (CDN)
- Google Fonts (Outfit)
