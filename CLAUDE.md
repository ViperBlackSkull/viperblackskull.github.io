# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based personal portfolio website for Simon Nolet, a cybersecurity professional. The site features a Matrix-themed design with a bilingual interface (English/French) showcasing professional experience, presentations, research, and contributions to the cybersecurity community.

## Tech Stack

- **Static Site Generator**: Jekyll (configured in `_config.yml`)
- **Framework**: Bootstrap 4.5.2
- **Styling**: Custom CSS with Matrix-themed design (black background, green text)
- **JavaScript**: Vanilla JS for language toggle and Matrix code rain effect
- **Hosting**: GitHub Pages (as indicated by the repository name ending in `.github.io`)
- **Language Support**: Bilingual (English/French) with client-side translation

## File Structure

- `index.html` - Main portfolio page with complete profile information and enhanced content
- `index2.html` - Alternative version with slightly different styling and simplified content
- `matrix.html` - (Referenced but content not analyzed)
- `_config.yml` - Jekyll configuration with theme and title settings
- `img/simon.jpg` - Profile image

## Key Features

### Bilingual Support
The site implements client-side language switching between English and French. Content translation is handled via JavaScript in the `toggleLanguage()` function, which dynamically updates text content for each section.

### Matrix Animation
Both versions include a animated Matrix code rain effect implemented with HTML5 Canvas, creating falling green characters in the background.

### Responsive Design
Uses Bootstrap 4 grid system and responsive classes for mobile compatibility.

## Common Development Tasks

### Adding New Presentations
To add a new presentation (as requested for https://www.youtube.com/watch?v=J6EiHTx9_dQ&ab_channel=HackfestCommunication):

1. **English version**: Add new `<li>` element to the presentations list in HTML
2. **French version**: Add corresponding entry to the French translation in the `toggleLanguage()` function
3. **Format**: `<li><a href="URL">Title</a> (Date - Event)</li>`

The presentations are stored in two places:
- Static HTML in the presentations section
- Dynamic French translations in the JavaScript `toggleLanguage()` function around lines 164-175

### Updating Content
- **Profile sections**: Modify HTML directly for English, update JavaScript for French translations
- **Styling**: Update the `<style>` block in the `<head>` section
- **New sections**: Add HTML structure and corresponding translations in JavaScript

### Jekyll Configuration
- Theme: jekyll-theme-cayman
- Title: Simon Nolet's Portfolio
- Runs on: self-hosted

## Testing

Since this is a static Jekyll site, testing involves:
1. **Local Jekyll server**: `bundle exec jekyll serve` (if Jekyll is installed)
2. **GitHub Pages deployment**: Push to master branch for automatic deployment
3. **Manual testing**: Open HTML files directly in browser for quick validation

## Content Guidelines

The site focuses on cybersecurity education and professional expertise, specifically:
- Offensive security and penetration testing
- CTF challenge design and education
- Community contributions and volunteering
- Professional presentations and research
- Maintaining bilingual accessibility

When adding content, ensure both English and French versions are provided to maintain the bilingual nature of the site.