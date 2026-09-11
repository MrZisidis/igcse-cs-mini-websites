# Project Organization & Improvement Plan

## Current State Analysis
- **Structure**: Flat directory with independent HTML files.
- **Technology**: HTML5, Tailwind CSS (via CDN), Vanilla JavaScript.
- **Styling**: Consistent use of Tailwind for layout and aesthetics.
- **Redundancy**: Header (Navigation) and Footer code is duplicated across `index.html` and sub-pages (e.g., `python_turtle_revision.html`). This makes updating links or styles difficult as it requires editing every file.

## Proposed Organization Steps

### 1. Cleanup
- [ ] Move `index_OLD.html` to an `_archive/` directory to declutter the root.
- [ ] Ensure all filenames follow a consistent naming convention (currently mixed `kebab-case` and `snake_case` e.g., `python-rev-lists-sorting.html` vs `log_analyser.html`).

### 2. Structural Improvements (Refactoring)
- **Shared Components**: Create a simple JavaScript system to inject the **Header** and **Footer** dynamically.
  - *Benefit*: You only change the menu in one place, and it updates everywhere.
- **Assets Folder**: Create `assets/js`, `assets/css` directory structure for any custom scripts or global styles.

### 3. SEO & Metadata
- Ensure all pages have unique `<title>` and `<meta name="description">` tags.
- Verify Open Graph (OG) tags for nice sharing on social media/Teams/Google Classroom.

## Workflow for New Content
1. Duplicate a "Template" file (which we can create).
2. Update the main content area.
3. Add the link to `index.html` (or the `projects.js` data file if we automate the index page).
