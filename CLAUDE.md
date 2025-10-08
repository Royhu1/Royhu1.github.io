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

## Resume and Website Sync Rules

**IMPORTANT**: When updating the resume, ALWAYS update both files in sync:

1. **Markdown Resume**: `resume/resume.md`
2. **Website Homepage**: `index.html`

### Update Workflow

When adding new content to the resume (e.g., new experience, publications, awards):

1. **Update Markdown Resume**:
   - Edit `resume/resume.md`
   - Follow the version control system (see below)

2. **Update Website Homepage**:
   - Edit corresponding section in `index.html`
   - Update navigation if adding new sections
   - Adjust CSS if needed in `css/style.css`

3. **Version Control**:
   - Backup current version: `cp resume/resume.md resume/versions/resume_v{X}.{Y}_{DATE}.md`
   - Update `resume/VERSION_HISTORY.md` with changes
   - Commit both files together

### Example: Adding Teaching Experience

```bash
# 1. Backup current version
cp resume/resume.md resume/versions/resume_v1.0_2024-10-08.md

# 2. Edit resume/resume.md - add Teaching Experience section

# 3. Edit index.html - add Teaching section and nav link

# 4. Update VERSION_HISTORY.md

# 5. Commit all changes together
git add resume/ index.html css/
git commit -m "feat: Add teaching experience to resume and website"
git push
```

## Common Tasks

- **Add new pages**: Create new HTML files in the root directory
- **Update content**: Edit HTML files directly AND update `resume/resume.md` if it's resume-related
- **Add styling**: Create CSS files and link them in HTML
- **Add interactivity**: Add JavaScript files
- **View changes**: Push to GitHub and wait for deployment, or test locally with a local server