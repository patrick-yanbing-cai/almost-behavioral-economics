# Almost Behavioral Economics

Almost Behavioral Economics is a bilingual, open, reproducible learning project in behavioral economics.

The reproducible course materials are not available yet; the current repository prepares the structure for them.

## Access the Project

Read online:

- Website: https://patrick-yanbing-cai.github.io/almost-behavioral-economics/
- Chinese entry: https://patrick-yanbing-cai.github.io/almost-behavioral-economics/zh/
- English entry: https://patrick-yanbing-cai.github.io/almost-behavioral-economics/en/

Repository:

- https://github.com/patrick-yanbing-cai/almost-behavioral-economics

Work locally:

```bash
git clone https://github.com/patrick-yanbing-cai/almost-behavioral-economics.git
cd almost-behavioral-economics
```

You can also download the repository as a ZIP file from the GitHub repository page.

## Current Status

The project is currently in its `v0.1-alpha` infrastructure stage.

The repository contains the bilingual Quarto site skeleton, navigation, placeholder Chapter 1 pages and notebooks, shared references, and license files. Substantive behavioral economics content has not been written yet.

## Repository and Website

This repository is the engineering and governance center for the project: source files, notebooks, references, build configuration, and licensing live here.

The website is the learner-facing entry point.

## Repository Structure

```text
zh/                 Chinese website pages and placeholder notebooks
en/                 English website pages and placeholder notebooks
src/yuki/           Minimal Python helper package skeleton
references.bib      Shared BibTeX references
_quarto.yml         Quarto website configuration
requirements.txt    Python dependencies for site/notebook infrastructure
LICENSE             MIT License for code
CONTENT-NOTICE.md   CC BY-SA 4.0 notice for educational content
```

## Local Use

The project is not yet available as a locally runnable course.

Local setup is currently useful for inspecting the repository and checking the site infrastructure:

```bash
python -m pip install -r requirements.txt
quarto render
```

Quarto must be installed separately.

## Notebooks

Chapter 1 notebook files are currently placeholders. Running and reproducing substantive notebook materials will be documented once the first course content is written.

## Contributing

This project is not yet at a general contribution stage.

For now, changes should stay limited to explicitly scoped infrastructure, documentation, translation, or review tasks. Substantive behavioral economics content should not be added unless a dedicated issue defines the scope.

## License

Unless otherwise noted, educational content is licensed under CC BY-SA 4.0. See `CONTENT-NOTICE.md`.

Code is licensed under the MIT License. See `LICENSE`.
