# Python Installation Support - Onboarding Guide

This is a Quarto-based documentation project for the Python Installation Support team onboarding guide.

## Features

- 📄 Export to multiple formats (HTML, PDF, DOCX)
- 🌐 GitHub Pages deployment
- 🎨 Responsive web design
- 📱 Mobile-friendly layout

## Usage

### Local Development

```bash
# Render main formats (HTML, PDF, DOCX)
quarto render index.qmd --to html
quarto render index.qmd --to pdf  
quarto render index.qmd --to docx

# Render slides separately (due to LaTeX conflicts)
quarto render index.qmd --to beamer

# Render all main formats at once (excludes beamer)
quarto render --to html,pdf,docx

# Preview in browser
quarto preview
```

### Output Files

After rendering, you'll find:
- `docs/index.html` - Web version
- `docs/index.pdf` - PDF version
- `docs/index.docx` - Word document version
- `docs/index.beamer.pdf` - Beamer slides (from index.qmd)

### GitHub Pages

The site automatically deploys to GitHub Pages when you push to the main branch. The workflow is configured in `.github/workflows/quarto-publish.yml`.

## Structure

```
quarto-onboarding/
├── _quarto.yml          # Quarto configuration
├── index.qmd            # Main content file
├── styles.css           # Custom styling
├── .github/
│   └── workflows/
│       └── quarto-publish.yml  # GitHub Actions workflow
└── docs/                # Generated output files
```

## Customization

- Edit `index.qmd` to modify content
- Modify `styles.css` for custom styling
- Update `_quarto.yml` for configuration changes