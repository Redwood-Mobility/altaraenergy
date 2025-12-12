# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Altara Energy website - a Jekyll-based static site for a city convenience EV charging network. Hosted on GitHub Pages at altaraenergy.com.

**Brand positioning**: Standalone city charging brand, part of Pathfinder Rewards loyalty network. Operated by Rangeway (not prominently customer-facing). Focus on convenience, not premium/luxury.

## Build & Development Commands

```bash
# Install dependencies (from oldsite directory)
cd oldsite && bundle install

# Local development server
cd oldsite && bundle exec jekyll serve

# Build for production
cd oldsite && bundle exec jekyll build
```

The site builds automatically on GitHub Pages when pushed to main branch.

## Project Structure

The active site lives in `oldsite/` directory:

```
oldsite/
├── _config.yml          # Jekyll config, site metadata, organization info
├── _layouts/default.html # Base HTML template
├── _includes/
│   ├── header.html      # Nav, meta tags, structured data
│   └── footer.html      # Footer with links, social icons
├── assets/
│   ├── css/style.css    # All styles (includes dark mode)
│   └── js/main.js       # Mobile menu, smooth scroll
├── images/              # Logo variants, site images
└── *.html               # Page files (index, about, locations, etc.)
```

Root-level files (`ALTARA_WEBSITE_PROJECT_BRIEF.md`, `altara-brand-guidelines-v2.html`, `Logo/`) are reference materials, not part of the build.

## Key Configuration

**_config.yml** contains:
- Site metadata and SEO settings
- Organization contact info
- Social media links (@altaraev handles)
- Page-specific meta descriptions and keywords
- Tinylytics analytics ID

## Brand Guidelines

- **Colors**: Ocean Deep (#0A4B6E), Sunset Coral (#FF6B4A), system supports dark mode
- **Typography**: System font stack for performance
- **Logo files**: Located in `oldsite/images/` (altara-logo-horizontal.svg, altara-logo-small.svg)
- **Language**: Use "city" not "urban" in copy. Avoid premium/luxury positioning.

## Pages

- index.html - Homepage with hero, value props, CTA
- locations.html - Coming soon map, market list
- membership.html - Pathfinder Rewards tiers
- fleet.html - B2B fleet solutions
- partners.html - Site host recruitment
- about.html - Company mission
- faq.html - Common questions
- contact.html - Contact form

## Dependencies

- Jekyll 4.x
- jekyll-seo-tag plugin
- Font Awesome (CDN)
- Webrick (Ruby 3.0+ dev server)
