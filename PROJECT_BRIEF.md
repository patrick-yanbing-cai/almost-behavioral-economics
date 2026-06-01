# PROJECT_BRIEF.md

# Almost Behavioral Economics Engineering Brief

> Internal codename: **Yuki**
> Public project name: **Almost Behavioral Economics**
> Current working identity: **an open behavioral economics learning project**

---

## 1. Project Status

This document summarizes the current engineering and planning decisions for Almost Behavioral Economics.

The project is moving from conceptual planning to implementation. The next working environment will be Codex or a similar code-oriented agent. This brief should be treated as the current source of truth for repository setup, website structure, bilingual architecture, release planning, and agent collaboration.

Specific notebook content is intentionally not finalized here. The first content module will be Chapter 1 on reference-dependent preferences, but detailed notebook writing will be handled separately.

---

## 2. Core Project Identity

Almost Behavioral Economics is an open learning project in behavioral economics.

It is not primarily a computational economics project. Code, notebooks, visualizations, and numerical experiments are used only when they help readers understand theoretical ideas, model failures, or conceptual transitions.

The core of the project is:

* structured learning;
* economic intuition;
* model-based reasoning;
* clear theoretical narratives;
* high-quality bilingual presentation;
* open-source publication.

The project should be positioned for economics students who want to systematically enter modern behavioral economics beyond textbook-level summaries and scattered popular examples.

---

## 3. Internal Codename and Public Naming

### Internal codename

The internal codename is:

```text
Yuki
```

This can be used for internal repo naming, Trello/GitHub project tracking, and agent workflow references.

### Public name

The public project name is:

```text
Almost Behavioral Economics
```

Yuki remains the internal codename for repo planning and agent workflow references.

### Preface / manifesto title

The phrase:

```text
What We Care About: Behavioral Economics
```

should be preserved as a possible preface, manifesto, or opening essay title.

It has a useful double meaning:

1. what we intellectually care about is behavioral economics;
2. “what people care about” is itself a core behavioral economics question involving preferences, attention, reference points, welfare, beliefs, and utility.

It should not be used as the main website name for now because it is too long and book-like.

---

## 4. Market Positioning

The external-facing message should focus on user need rather than the author’s personal motivation.

The project should make a potential reader think:

```text
This is a structured open learning project that can help me seriously learn behavioral economics.
```

Recommended positioning sentence:

```text
This is a bilingual open learning project in behavioral economics for economics students who want to understand how modern behavioral models revise, extend, and challenge standard models of choice.
```

Chinese version:

```text
这是一个中英双语的行为经济学开源学习项目，面向希望系统进入现代行为经济学的经济学学习者，帮助读者理解行为模型如何修正、扩展并挑战标准选择模型。
```

---

## 5. Bilingual Architecture

The project will maintain Chinese and English as separate language versions.

The structure should not be same-page bilingual. Instead, the website should have two parallel versions:

```text
/zh/
/en/
```

A language switch should appear in the top-right navigation area.

### Language design

Chinese and English should be fully separated at the page level.

The Chinese version is not merely an informal translation of the English version. It should be written for Chinese economics students.

The English version should be written cleanly and professionally so that the project is understandable to the broader open education community.

### Language switch

Initial implementation can use a simple language switch:

```text
中文 | English
```

First-stage implementation may link to the language homepages:

```text
/zh/  <->  /en/
```

Later, page-level language switching can be implemented:

```text
/zh/ch01_overview.html  <->  /en/ch01_overview.html
/zh/notebooks/ch01_1a_expected_utility_failure.html  <->  /en/notebooks/ch01_1a_expected_utility_failure.html
```

---

## 6. Technical Stack

The first-stage technical stack is fixed as:

```text
Python
Jupyter Notebook
Quarto
GitHub
GitHub Pages
GitHub Actions
BibTeX
```

### Quarto

Use Quarto as a website publishing layer.

The project should be implemented as a Quarto website, not a Quarto book.

Reason:

* the project is an open learning website rather than a finished linear book;
* sidebar navigation is important;
* modules, docs, protocols, and future materials should be easy to add;
* bilingual site structure is easier to manage as a website.

### Notebook format

Use `.ipynb` for core notebooks.

Quarto should render the notebooks into HTML pages.

### References

Use BibTeX via a shared file:

```text
references.bib
```

---

## 7. Repository Structure

Use the following repository structure:

```text
project-yuki/
│
├── README.md
├── README.zh.md
├── LICENSE
├── requirements.txt
├── references.bib
├── _quarto.yml
│
├── zh/
│   ├── index.qmd
│   ├── ch01_overview.qmd
│   ├── notebooks/
│   │   ├── ch01_1a_expected_utility_failure.ipynb
│   │   ├── ch01_1b_kt_exogenous_reference_points.ipynb
│   │   ├── ch01_1c_kr_expectations_news_utility.ipynb
│   │   └── ch01_1d_probability_weighting.ipynb
│   └── docs/
│       ├── glossary.qmd
│       ├── references.qmd
│       └── production_protocol.qmd
│
├── en/
│   ├── index.qmd
│   ├── ch01_overview.qmd
│   ├── notebooks/
│   │   ├── ch01_1a_expected_utility_failure.ipynb
│   │   ├── ch01_1b_kt_exogenous_reference_points.ipynb
│   │   ├── ch01_1c_kr_expectations_news_utility.ipynb
│   │   └── ch01_1d_probability_weighting.ipynb
│   └── docs/
│       ├── glossary.qmd
│       ├── references.qmd
│       └── production_protocol.qmd
│
├── src/
│   └── yuki/
│       ├── __init__.py
│       ├── utility.py
│       ├── plotting.py
│       ├── experiments.py
│       └── widgets.py
│
└── .github/
    └── workflows/
        └── publish.yml
```

### Notes

* `zh/` and `en/` are parallel language sites.
* `src/yuki/` stores reusable Python code.
* `references.bib` is shared across both language versions.
* `README.md` is the English GitHub README.
* `README.zh.md` is the Chinese GitHub README.
* Website pages should be rendered by Quarto and deployed through GitHub Actions.

---

## 8. Website Structure

The Quarto website should use sidebar navigation.

The website should feel like a structured learning project, not a collection of files.

### Suggested sidebar structure

```text
Home
├── Start Here
├── Chapter 1: Reference-Dependent Preferences
│   ├── Overview
│   ├── 1a. The Failure of Expected Utility
│   ├── 1b. Building Reference Points
│   ├── 1c. Endogenizing Reference Points
│   └── 1d. Probability Weighting
├── Glossary
├── References
└── Production Protocol
```

The Chinese version should use Chinese page titles.

The English version should use English page titles.

---

## 9. README vs Website Homepage

README and website homepage have different roles.

### README

README is for:

* GitHub visitors;
* potential contributors;
* technical reviewers;
* future collaborators;
* people checking project status and build instructions.

README should include:

```text
Project description
Website links
Current status
Repository structure
Local setup
How to build the website
How to run notebooks
Contribution notes
License
```

README should be concise and practical.

It should not serve as the main teaching entry.

### Website homepage

The website homepage is for learners.

It should answer:

```text
What is this project?
Who is it for?
Where should I start?
What is currently available?
How do I read or run the materials?
How do I switch languages?
```

The homepage should function like a course landing page.

---

## 10. Website Homepage Wireframe

Use this as the first-stage homepage structure.

### Section 1: Hero

English:

```markdown
# Almost Behavioral Economics

A bilingual open learning project for modern behavioral economics.

This project helps economics students understand how behavioral economics revises, extends, and challenges standard models of choice.
```

Chinese:

```markdown
# Almost Behavioral Economics

一个面向现代行为经济学的中英双语开源学习项目。

本项目帮助经济学学习者理解行为经济学如何修正、扩展并挑战标准选择模型。
```

Buttons:

```text
Start with Chapter 1
View on GitHub
Read the Preface
```

Chinese buttons:

```text
从 Chapter 1 开始
查看 GitHub
阅读前言
```

### Section 2: Who This Is For

English:

```markdown
## Who is this for?

This project is designed for economics students who want to move beyond textbook-level introductions and understand behavioral economics through structured narratives, models, and guided experiments.
```

Chinese:

```markdown
## 这个项目适合谁？

本项目面向希望超越教材式简介、系统理解行为经济学理论推进的经济学学习者。读者最好具备基础微观经济学、基本概率知识，并愿意阅读模型、例子和少量代码实验。
```

### Section 3: Current Module

English:

```markdown
## Current Module: Chapter 1

Reference-Dependent Preferences

1. The Failure of Expected Utility
2. Building Reference Points
3. Endogenizing Reference Points
4. Probability Weighting
```

Chinese:

```markdown
## 当前模块：Chapter 1

参考依赖偏好

1. EU 的失败
2. 参考点的初步建立
3. 参考点的内生化
4. Probability Weighting
```

### Section 4: How to Use This Project

English:

```markdown
## How to Use This Project

You can use this project in three ways:

1. Read the materials online as structured lecture notes.
2. Run selected experiments in Google Colab.
3. Clone the GitHub repository and reproduce the notebooks locally.
```

Chinese:

```markdown
## 如何使用这个项目

你可以用三种方式使用本项目：

1. 直接在线阅读；
2. 使用 Google Colab 运行部分实验；
3. 克隆 GitHub 仓库，在本地完整复现。
```

### Section 5: How This Project Is Produced

English:

```markdown
## How This Project Is Produced

This project uses a human-led, agent-assisted workflow. Human editors control the theoretical structure, narrative, and final review. AI agents assist with drafting, code implementation, translation, review, and technical maintenance.
```

Chinese:

```markdown
## 项目如何生产

本项目采用 human-led, agent-assisted 的工作方式。人类作者负责理论结构、叙事判断和最终审稿；AI agents 协助完成初稿、代码实现、翻译、审稿和工程维护。
```

---

## 11. Chapter 1 Scope

The first-stage content module is:

```text
Chapter 1: Reference-Dependent Preferences
```

This corresponds to the first major module of the project.

The module contains four notebooks:

```text
ch01_1a_expected_utility_failure.ipynb
ch01_1b_kt_exogenous_reference_points.ipynb
ch01_1c_kr_expectations_news_utility.ipynb
ch01_1d_probability_weighting.ipynb
```

### Notebook 1a

```text
EU 的失败
The Failure of Expected Utility
```

Main idea:

```text
Expected utility can explain risk aversion, but it struggles with ordinary small-stakes risk attitudes and systematic choice reversals.
```

### Notebook 1b

```text
参考点的初步建立
Building Reference Points: Kahneman-Tversky and Exogenous Reference Point Applications
```

Main idea:

```text
Kahneman-Tversky introduces reference points, gains, losses, and loss aversion. This shifts the analysis from final wealth levels to changes relative to a reference point.
```

### Notebook 1c

```text
参考点的内生化
Endogenizing Reference Points: Kőszegi-Rabin, Expectations, and News Utility
```

Main idea:

```text
Kőszegi-Rabin endogenizes the reference point as expectations and extends reference dependence into a broader economic framework, including news utility.
```

### Notebook 1d

```text
概率加权
Probability Weighting
```

Main idea:

```text
People may not process probabilities linearly. Probability weighting explains systematic deviations from expected utility that are not captured by loss aversion alone.
```

### Structural rule

Each notebook should have its own main storyline.

Each notebook should be readable on its own.

Related links should be chosen by conceptual relevance, not by mechanical sequence.

---

## 12. Code Philosophy

The project should not be framed as computational behavioral economics.

Code is a teaching instrument.

Use code only when it improves understanding.

### Code should be used for:

```text
guided experiments
parameter exploration
visualizing model implications
showing where a model fails
helping readers test intuition
```

### Code should not be used for:

```text
displaying technical sophistication
turning the project into a software package
making simple concepts unnecessarily computational
replacing theoretical explanation
```

### Rule of thumb

If a code block only produces a fixed output and readers have no reason to modify it, consider replacing it with a static figure or prose explanation.

If a code block lets readers explore a model boundary, test a parameter, or experience a failed attempt to rescue a standard model, it is likely useful.

---

## 13. Notebook Runtime Design

The project should support three levels of use:

### Reader

Reads the rendered website pages only.

No Python setup required.

### Runner

Uses Google Colab to run selected notebooks or experiments.

Each notebook should eventually include a Colab badge.

### Contributor

Clones the GitHub repository and runs the project locally.

The README should include local setup instructions.

### First-stage runtime support

Support:

```text
Web reading
Google Colab
Local reproduction
```

Do not support Binder in the first stage unless there is a strong reason later.

---

## 14. Agent Collaboration Model

The project uses a fixed multi-agent collaboration model.

### Human Editor-in-Chief

Responsible for:

```text
theoretical judgment
notebook storyline
model selection
quality control
final review
release decision
```

### ChatGPT: Editorial and Pedagogy Agent

Responsible for:

```text
notebook outline
pedagogical structure
theoretical explanation
reader difficulty diagnosis
storyline review
bilingual phrasing review
release checklist reminders
```

### Codex: Code and Infrastructure Agent

Responsible for:

```text
repository setup
Quarto configuration
GitHub Actions
Jupyter notebook skeleton
Python implementation
plotting functions
widgets
dependency management
local build instructions
render/debug workflow
```

### DeepSeek: Chinese Production and Second-review Agent

Responsible for:

```text
Chinese explanation drafts
alternative phrasings
glossary drafts
exercise drafts
social media summaries
Chinese fluency review
second-pass clarity review
```

### Harness engineering

The agent workflow should not be understood only as prompt engineering.

The project should gradually develop harness engineering:

```text
templates
checklists
scripts
review protocols
notebook skeletons
automated builds
validation steps
source maps
release routines
```

---

## 15. Source Map

Each notebook should include a source map.

A source map is a structured record of:

```text
which theories come from which papers or handbook chapters
which examples come from the literature
which examples are original
which numerical experiments are original implementations
which figures are project-generated
```

Purpose:

```text
academic transparency
copyright safety
reader trust
clear separation between literature and project-original teaching design
```

Example format:

```markdown
## Source Map

| Component | Source | Role in this notebook |
|---|---|---|
| Expected utility framework | Standard microeconomic theory | Baseline model |
| Rabin calibration theorem | Rabin (2000) | Core theoretical result |
| Small-stakes risk aversion discussion | Handbook of Behavioral Economics, Chapter 1 | Interpretive frame |
| Allais paradox | Allais (1953) | Choice anomaly |
| Interactive calibration experiment | Almost Behavioral Economics original implementation | Teaching experiment |
| Figures and code | Almost Behavioral Economics original implementation | Visualization and computation |
```

---

## 16. Citation and References

Use BibTeX.

Shared file:

```text
references.bib
```

Quarto should use this file for citations in both language versions.

Each notebook should include:

```text
references section
source map
citation keys connected to references.bib
```

---

## 17. License

The project should use a dual-license structure.

### Educational content

Use:

```text
CC BY-SA 4.0
```

For:

```text
text
figures
teaching explanations
learning materials
website content
```

Meaning:

* others can share and adapt the content;
* they must give attribution;
* adapted versions must use the same license.

### Code

Use:

```text
MIT License
```

For:

```text
Python code
notebook code cells
Quarto configuration
scripts
```

Meaning:

* others can freely use, modify, distribute, and even use commercially;
* they must preserve the copyright and license notice.

### README license statement

Use something like:

```markdown
## License

Unless otherwise noted, the educational content in this repository is licensed under CC BY-SA 4.0.

All code in this repository is licensed under the MIT License.
```

---

## 18. GitHub Project Management

Use GitHub only.

Do not maintain a separate Trello board once the project moves into implementation.

GitHub should handle:

```text
issues
milestones
pull requests
release notes
project planning
deployment status
documentation
```

The repo is not merely an entrance page. It is the engineering and governance center of the project.

The website is the learner-facing entrance.

---

## 19. Release Planning

The first release can happen after notebook 1a is completed.

### Release condition for v0.1-alpha

```text
Quarto website builds successfully
zh/en site structure exists
homepage exists
Chapter 1 overview exists
1a notebook exists
1a can render to HTML
1a has Colab link or placeholder
references.bib exists
glossary page exists
source map exists for 1a
README.md and README.zh.md exist
GitHub Actions deployment works
```

### Release vs publicity

Release and publicity are separate.

The project can have a technical release before any major public promotion.

Promotion strategy will be decided separately.

---

## 20. Human Review Checklist

Before releasing any notebook, complete the following checklist.

### Theory check

```text
Are the key concepts defined accurately?
Are the model assumptions explicit?
Does the explanation overstate the model?
Does the text distinguish descriptive, normative, and welfare claims?
Does the text avoid unsupported causal claims?
Does the text avoid saying behavioral economics simply “overthrows” standard economics?
Has the explanation been checked against the original literature or handbook?
```

### Narrative check

```text
Does the notebook have one clear core question?
Does the opening problem motivate the theory?
Does every section serve the main storyline?
Are there unnecessary background digressions?
Can a reader state the notebook’s main conclusion after reading?
Is there a clear aha moment?
Does the ending point to genuinely related material without making the notebook dependent on it?
```

### Code check

```text
Can the notebook run from top to bottom?
Are there hidden state dependencies?
Do code outputs match the written explanation?
Is each code block pedagogically necessary?
Are default parameter values reasonable?
Are errors understandable?
Does the notebook run in Colab if Colab is supported?
```

### Bilingual check

```text
Do the zh/en titles correspond?
Are key terms translated consistently?
Has the glossary been updated?
Are references consistent across zh/en?
Does the English version preserve important qualifications?
Does the Chinese version avoid excessive informality?
```

### Engineering check

```text
Does Quarto render successfully?
Does the sidebar link correctly?
Does the language switch work?
Does the Colab badge work or clearly say coming soon?
Does GitHub Actions pass?
Do filenames follow the naming convention?
Are release notes updated?
```

### Source and license check

```text
Are all core references cited?
Does the notebook avoid copying source text?
Are figures original or properly attributed?
Is code original or properly attributed?
Is the source map complete?
Are license statements clear?
```

---

## 21. Open Decisions

The following issues remain unresolved.

### Website visual design

Need later decisions on:

```text
theme
typography
color
logo
figure style
Chinese font handling
mobile readability
```

### Notebook template

Use the canonical template in `NOTEBOOK_TEMPLATE.md`.

Standard English section structure:

```text
Title
Colab support marker
Abstract
Learning Goals
Prerequisites
Opening Problem
Baseline Model
Key Tension
Core Idea
Guided Example / Experiment
What This Teaches Us
Key Takeaways
Glossary
Source Map
References
Related
```

### Chapter overview template

Need to decide exact structure.

Possible components:

```text
chapter motivation
roadmap
conceptual arc
notebook links
how to read this chapter
key references
```

### Code and visualization style

Need later decisions on:

```text
matplotlib vs plotly
ipywidgets or alternatives
how much code to expose
whether helper functions should be hidden
beginner-friendly code vs package-style code
```

### Public preface

Need to write later:

```text
What We Care About: Behavioral Economics
```

This should explain the intellectual motivation of the project, but it is not required for the first engineering setup.

---

## 22. Immediate Next Steps for Codex

Codex should begin with engineering setup, not notebook content.

### Step 1: Initialize repository structure

Create the directory and file structure described above.

### Step 2: Create Quarto website skeleton

Set up:

```text
_quarto.yml
zh/index.qmd
en/index.qmd
zh/ch01_overview.qmd
en/ch01_overview.qmd
zh/docs/glossary.qmd
en/docs/glossary.qmd
zh/docs/references.qmd
en/docs/references.qmd
zh/docs/production_protocol.qmd
en/docs/production_protocol.qmd
```

### Step 3: Configure sidebar navigation

Create separate sidebar entries for zh and en.

Ensure the website has:

```text
Home
Chapter 1
Glossary
References
Production Protocol
```

### Step 4: Add placeholder notebooks

Create placeholder notebook files:

```text
zh/notebooks/ch01_1a_expected_utility_failure.ipynb
zh/notebooks/ch01_1b_kt_exogenous_reference_points.ipynb
zh/notebooks/ch01_1c_kr_expectations_news_utility.ipynb
zh/notebooks/ch01_1d_probability_weighting.ipynb

en/notebooks/ch01_1a_expected_utility_failure.ipynb
en/notebooks/ch01_1b_kt_exogenous_reference_points.ipynb
en/notebooks/ch01_1c_kr_expectations_news_utility.ipynb
en/notebooks/ch01_1d_probability_weighting.ipynb
```

### Step 5: Add basic README files

Create:

```text
README.md
README.zh.md
```

README should include:

```text
project description
website links placeholder
current status
repository structure
local setup
Quarto build instructions
license statement
```

### Step 6: Add shared references file

Create:

```text
references.bib
```

with placeholder entries for:

```text
Allais (1953)
Rabin (2000)
Kahneman and Tversky (1979)
Kőszegi and Rabin
Handbook of Behavioral Economics
```

Exact BibTeX entries can be refined later.

### Step 7: Add Python package skeleton

Create:

```text
src/yuki/__init__.py
src/yuki/utility.py
src/yuki/plotting.py
src/yuki/experiments.py
src/yuki/widgets.py
```

Keep files minimal for now.

### Step 8: Add requirements.txt

Include only minimal dependencies at first:

```text
jupyter
numpy
pandas
matplotlib
ipywidgets
quarto-related dependencies if needed
```

Do not over-expand dependencies.

### Step 9: Add GitHub Actions deployment

Create:

```text
.github/workflows/publish.yml
```

to render the Quarto website and deploy to GitHub Pages.

### Step 10: Verify local render

The project should support:

```bash
quarto render
```

and ideally:

```bash
quarto preview
```

### Step 11: Prepare v0.1-alpha milestone

Create GitHub milestone:

```text
v0.1-alpha: 1a website prototype
```

with issues for:

```text
repo skeleton
Quarto site skeleton
zh/en homepage
Chapter 1 overview
1a notebook prototype
references.bib
glossary
source map template
GitHub Actions deployment
README files
license setup
```

---

## 23. Non-goals for the First Engineering Pass

Do not do the following in the first setup pass:

```text
Do not revisit the public project name.
Do not design a logo.
Do not write full notebook content.
Do not over-engineer Python package structure.
Do not add Binder.
Do not build a full book.
Do not create complex interactive frontends.
Do not optimize visual design prematurely.
Do not write social media materials.
Do not expand beyond Chapter 1.
```

The immediate goal is:

```text
A clean bilingual Quarto website skeleton with GitHub deployment and placeholder Chapter 1 structure.
```

---

## 24. Current Engineering Conclusion

The project should now move into implementation with the following guiding principle:

```text
Build the smallest serious version of the project infrastructure first.
```

That means:

```text
clear repo structure
zh/en separation
Quarto website with sidebar
GitHub Actions deployment
README files
license structure
references.bib
placeholder Chapter 1 module
minimal Python package skeleton
```

Only after the infrastructure skeleton works should the project move into detailed writing of notebook 1a.
