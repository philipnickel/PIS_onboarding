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
# Render all formats
quarto render

# Render specific format
quarto render --to html
quarto render --to pdf
quarto render --to docx

# Preview in browser
quarto preview
```

### Output Files

After rendering, you'll find:
- `docs/index.html` - Web version
- `docs/index.pdf` - PDF version
- `docs/index.docx` - Word document version

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