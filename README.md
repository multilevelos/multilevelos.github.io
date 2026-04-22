# MMLoS Website

This repository contains the website for the **Multi-Modal Level of Service (MMLoS)** research project.

## Site Structure

```
multilevelos.github.io/
├── _quarto.yml        # Quarto configuration
├── index.qmd          # Home page
├── about.qmd          # Project overview
├── team.qmd           # Project team
├── approach.qmd       # Methodology
├── research.qmd       # Research & literature
├── tools.qmd          # Tools & datasets
├── updates.qmd        # News & milestones
├── 404.qmd            # Error page
├── references.bib     # Bibliography (37 entries)
├── styles.scss        # Custom SCSS styling
└── files/             # Images and assets
    └── images/
        ├── mmlos-logo.svg  # Project logo
        └── logo.svg        # Avatar
```

## Development

### Local preview

```bash
cd ~/github/multilevelos/multilevelos.github.io
quarto preview
```

### Render to static site

```bash
quarto render
```

Output goes into `_site/`.

## Deployment

This site is deployed to GitHub Pages automatically via GitHub Actions on every push to the `main` branch.

**Workflow file:** [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml)

The workflow:
1. Checks out the repository
2. Sets up Quarto and R
3. Renders all `.qmd` files to HTML
4. Pushes the `_site/` output to the `main` branch of this repo (which GitHub Pages serves)

No manual deployment steps needed — just commit and push.

## Technologies

- [Quarto](https://quarto.org) — publishing system
- [GitHub Actions](https://github.com/features/actions) — CI/CD
- [GitHub Pages](https://pages.github.io) — hosting
- SCSS → CSS custom styling

## Project Info

**Project:** MMLoS — Multi-Modal Level of Service  
**Funded by:** Active Travel England  
**Duration:** April 2026 – September 2027  
**Lead institutions:** University of Westminster (Active Travel Academy), University of Leeds (Institute for Transport Studies)

For project details, see the [About](/about.qmd) page.
