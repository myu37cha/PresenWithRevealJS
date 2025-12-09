# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for hosting Reveal.js presentation slides, deployed via GitHub Pages. Each HTML file in the repository is a standalone Reveal.js presentation.

## Architecture

- **No build system**: Pure static HTML files using Reveal.js from CDN
- **Reveal.js v5**: Loaded from `https://cdn.jsdelivr.net/npm/reveal.js@5/`
- **Presentations**: Each `.html` file is an independent presentation (e.g., `hamanako_reveal.html`)
- **Hosting**: GitHub Pages serves the files directly

## Creating New Presentations

New presentations should follow this structure:
1. Create an HTML file in the repository root
2. Use Reveal.js CDN for CSS and JS (see existing files for template)
3. Include `<div class="reveal"><div class="slides">` structure
4. Initialize Reveal with `Reveal.initialize()` in a script tag

## Local Development

Open any HTML file directly in a browser to preview. No server required.

## Reveal.js Configuration

Current presentations use these standard settings:
- `hash: true` - URL fragments for slide navigation
- `slideNumber: true` - Show slide numbers
- `transition: 'fade'` - Fade transition between slides
- `center: true` - Vertically center content
