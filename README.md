# Almost Behavioral Economics

Almost Behavioral Economics is a bilingual open learning project in behavioral economics. Project Yuki remains the internal codename.

This repository currently contains infrastructure only: a Quarto website skeleton, bilingual page structure, placeholder Chapter 1 notebooks, shared references, and a minimal Python package namespace.

## Website

GitHub Pages URL: to be configured after repository publication.

Language entry points:

- `zh/`
- `en/`

## Current Status

Infrastructure skeleton initialized. Substantive economics content has not been written.

## Repository Structure

```text
zh/                 Chinese website pages and notebooks
en/                 English website pages and notebooks
src/yuki/           Minimal Python helper package skeleton
references.bib      Shared BibTeX references
_quarto.yml         Quarto website configuration
```

## Local Setup

Install Python dependencies:

```bash
python -m pip install -r requirements.txt
```

Install Quarto separately from the official Quarto distribution.

## Build the Website

```bash
quarto render
```

Preview locally:

```bash
quarto preview
```

## Run Notebooks

Open notebooks from `zh/notebooks/` or `en/notebooks/` in Jupyter:

```bash
jupyter notebook
```

## Contributing

Use focused changes. Infrastructure, content, translation, and review work should be kept separate when possible.

## License

Unless otherwise noted, educational content in this repository is intended to be licensed under CC BY-SA 4.0.

All code in this repository is intended to be licensed under the MIT License.
