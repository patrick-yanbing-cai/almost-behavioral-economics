# Notebook Template

This document is the canonical v0 template for Chapter 1 notebooks. Use it when creating or revising any notebook in `en/notebooks/` or `zh/notebooks/`.

The template is a writing scaffold, not a content outline for a specific lesson. Keep notebook sections structurally aligned across languages, but write headings and placeholder text naturally in each language.

## English Template

```markdown
# Title

> Colab support: coming soon.

## Abstract

## Learning Goals

## Prerequisites

## Opening Problem

## Baseline Model

## Key Tension

## Core Idea

## Guided Example / Experiment

## What This Teaches Us

## Key Takeaways

## Glossary

## Source Map

## References

## Related
```

## Chinese Template

```markdown
# 标题

> Colab 支持：即将提供。

## 本节概述

## 学习目标

## 预备知识

## 开场问题

## 基准模型

## 核心张力

## 核心思路

## 引导例子 / 实验

## 理解的推进

## 本节要点

## 术语表

## 来源地图

## 参考文献

## 相关内容
```

## Section Rules

- Each notebook should have one clear main question and its own main storyline.
- Each notebook should be readable on its own. Do not rely on the reader having read the previous notebook or immediately reading the next notebook.
- Use the fixed top-level section order above. Add local subsections only when they serve the notebook's main question.
- Use `Related` / `相关内容` for conceptually relevant links. Do not add a next-notebook link unless it is genuinely relevant.
- `Learning Goals` / `学习目标` should list 3-5 things the reader should be able to do after completing the notebook.
- `Prerequisites` / `预备知识` should briefly list useful concepts, math, coding skills, or prior notebooks.
- `Baseline Model` / `基准模型` should present the minimal benchmark needed for the notebook. Equations are optional and should appear only when they clarify the argument.
- `Key Tension` / `核心张力` should clarify the gap between the benchmark model and the phenomenon, behavior, question, or explanatory target.
- `Core Idea` / `核心思路` should state the explanatory move: a concept, mechanism, distinction, measurement idea, modeling direction, or bridge to another part of the chapter.
- `Guided Example / Experiment` / `引导例子 / 实验` may contain one example or a sequenced set of examples or experiments. It may use prose, tables, static numerical exercises, short code cells, or future widget placeholders.
- Do not add standalone `Exercises`, `Check Your Understanding`, `Implementation Notes`, `Code Notes`, or author-maintenance sections to learner notebooks.
- `What This Teaches Us` / `理解的推进` should explain the marginal understanding gained in the notebook.
- `Key Takeaways` / `本节要点` should list 3-5 concise takeaways.
- `Glossary` / `术语表` should list only key terms used in the notebook, with short local definitions and links to the site glossary.
- `References` / `参考文献` should list only sources cited, mentioned, or used in the notebook.

## Source Map Rules

Every notebook should include a structured source map. Source maps cover literature sources, examples adapted from literature, original examples, original numerical exercises, figures, code, widgets, simulations, and teaching design when relevant.

English source roles:

```text
core
support
extension
original
```

Chinese source roles:

```text
主线
支撑
延伸
原创
```

Role mapping:

| English | Chinese | Meaning |
|---|---|---|
| core | 主线 | Required for the notebook's main storyline |
| support | 支撑 | Helps explain an example, step, or transition |
| extension | 延伸 | Points to related material without expanding it here |
| original | 原创 | Project-generated teaching material |

English source map placeholder:

```markdown
| Component | Source | Source Role | Use in this notebook |
|---|---|---|---|
| Main theoretical claim | TBD | core | Establishes the notebook's central idea |
| Example or empirical pattern | TBD | support | Motivates or illustrates the key tension |
| Related extension | TBD | extension | Points to related material without expanding it here |
| Figure, code, simulation, or teaching design | Almost Behavioral Economics original implementation | original | Provides project-generated teaching material |
```

Chinese source map placeholder:

```markdown
| 组成部分 | 来源 | 来源角色 | 在本节中的用途 |
|---|---|---|---|
| 主要理论主张 | 待定 | 主线 | 建立本节的核心思路 |
| 例子或经验现象 | 待定 | 支撑 | 引出或说明核心张力 |
| 相关延伸 | 待定 | 延伸 | 指向相关材料，但不在本节展开 |
| 图表、代码、模拟或教学设计 | Almost Behavioral Economics 原创实现 | 原创 | 提供项目生成的教学材料 |
```
