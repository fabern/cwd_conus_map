# GECO Leaflet map template

A reusable [GECO](https://geco-group.org/) project template for building a single-page, full-screen Leaflet raster map with R and Quarto.

The included example provides:

- a full-viewport Leaflet map;
- a reproducible raster layer generated in R;
- a responsive, expandable information and references panel;
- GECO colours and branding; and
- a Quarto book project ready for GitHub Pages.

## Start a new project

1. Select **Use this template** on GitHub.
2. Choose an owner and a descriptive repository name.
3. Clone the new repository.
4. Replace the example title, text, references, and raster code in `index.qmd`.
5. Update the project title in `_quarto.yml`.

## Requirements

- [Quarto](https://quarto.org/docs/get-started/)
- R
- The R packages `leaflet` and `raster`

Install the R dependencies with:

```r
install.packages(c("leaflet", "raster"))
```

## Preview locally

From the project directory, run:

```bash
quarto preview
```

## Build

```bash
quarto render
```

The rendered website is written to `_site/`, which is intentionally excluded from version control.

## Publish with GitHub Pages

Publish the rendered project to the repository's `gh-pages` branch:

```bash
quarto publish gh-pages --no-browser
```

In the repository settings, configure **Pages → Build and deployment** to deploy from the `gh-pages` branch and its root directory.

## Project structure

```text
.
├── _quarto.yml          # Quarto book and HTML configuration
├── index.qmd            # Raster preparation, map, panel content and behaviour
├── styles.css           # Full-screen layout and GECO visual styling
├── images/
│   └── geco-logo.png    # GECO logo asset
└── README.md             # Template setup and publishing guide
```

## Attribution

The visual styling and logo treatment are adapted from the [GECO R book template](https://github.com/geco-bern/R_book_template).
