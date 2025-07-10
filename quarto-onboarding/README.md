# Python Installation Support - Onboarding Guide

This repository contains the onboarding guide for Python Installation Support team members, built with Quarto.

## Structure

- **contents/**: Individual content files for each section
  - `index.qmd`: Welcome page and navigation guide
  - `your-role.qmd`: Team responsibilities and workflow
  - `introduction-process.qmd`: Getting started and training
  - `tools-practicals.qmd`: Daily tools and procedures
- **fusion_steps/**: Step-by-step screenshots for FUSION time registration (also copied to contents/)
- **complete-guide.qmd**: Combined PDF version of all content using Quarto includes

## Development Commands

### Render All Documents
```bash
quarto render
```

### Render Individual Sections
```bash
quarto render contents/index.qmd
quarto render contents/your-role.qmd
quarto render contents/introduction-process.qmd
quarto render contents/tools-practicals.qmd
```

### Render Complete Guide PDF
```bash
quarto render complete-guide.qmd --to pdf
```

### Render HTML Only
```bash
quarto render --to html
```

## Automatic Content Sync

The complete guide PDF automatically includes content from all individual files using Quarto's `{{< include >}}` directive. The `complete-guide.qmd` file automatically:
- Includes all content from individual `.qmd` files  
- Combines everything into a single PDF
- Ensures the PDF always contains the latest content without manual updates

## Site Structure

The site uses:
- **Top navigation** (pinned, doesn't collapse)
- **Three main sections** with dedicated pages
- **Right sidebar** for "On this page" table of contents
- **External links** open in new tabs
- **Step-by-step images** for complex procedures
- **Complete PDF download** available from the home page

## Making Changes

1. Edit the individual content files in `contents/`
2. Run `quarto render` to update all HTML and PDF outputs

The complete guide PDF will automatically reflect any changes made to the individual content files through Quarto's include mechanism.