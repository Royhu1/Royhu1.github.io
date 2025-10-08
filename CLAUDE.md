# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a GitHub Pages repository for hosting a personal website at `Royhu1.github.io`. The site is currently minimal, containing only a basic "hello world" index.html file.

## File Structure

- `index.html` - Main entry point for the website (currently UTF-16 encoded)

## Development Commands

Since this is a static GitHub Pages site, no build process is required. Files are served directly.

To test locally:
```bash
# Serve the site locally (requires Python 3)
python -m http.server 8000

# Or with Python 2
python -m SimpleHTTPServer 8000

# Or with Node.js (if http-server is installed)
npx http-server .
```

## Deployment

Changes are automatically deployed to GitHub Pages when pushed to the main branch. The site will be available at `https://Royhu1.github.io`.

## File Encoding Note

The current `index.html` file is encoded in UTF-16 LE. For better compatibility and smaller file sizes, consider converting to UTF-8:

```bash
iconv -f utf-16le -t utf-8 index.html > index_utf8.html
mv index_utf8.html index.html
```

## Common Tasks

- **Add new pages**: Create new HTML files in the root directory
- **Update content**: Edit HTML files directly
- **Add styling**: Create CSS files and link them in HTML
- **Add interactivity**: Add JavaScript files
- **View changes**: Push to GitHub and wait for deployment, or test locally with a local server