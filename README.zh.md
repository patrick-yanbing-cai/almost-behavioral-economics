# Almost Behavioral Economics

Almost Behavioral Economics 是一个中英双语、开源、可复现的行为经济学学习项目。

可复现的课程材料尚未发布；当前仓库是在为这些材料准备结构。

## 获取项目

在线阅读：

- 网站首页：https://patrick-yanbing-cai.github.io/almost-behavioral-economics/
- 中文入口：https://patrick-yanbing-cai.github.io/almost-behavioral-economics/zh/
- 英文入口：https://patrick-yanbing-cai.github.io/almost-behavioral-economics/en/

GitHub 仓库：

- https://github.com/patrick-yanbing-cai/almost-behavioral-economics

本地获取：

```bash
git clone https://github.com/patrick-yanbing-cai/almost-behavioral-economics.git
cd almost-behavioral-economics
```

也可以在 GitHub 仓库页面下载 ZIP 文件。

## 当前状态

项目当前处于 `v0.1-alpha` 基础设施阶段。

本仓库包含中英双语 Quarto 网站骨架、导航结构、第 1 章占位页面和笔记本、共享参考文献与许可文件。实质性的行为经济学内容尚未编写。

## 仓库与网站

本仓库是项目的工程与治理中心：源文件、笔记本、参考文献、构建配置和许可文件都在这里维护。

网站是面向学习者的入口。

## 仓库结构

```text
zh/                 中文网站页面和占位笔记本
en/                 英文网站页面和占位笔记本
src/yuki/           最小 Python helper package 骨架
references.bib      共享 BibTeX 参考文献
_quarto.yml         Quarto 网站配置
requirements.txt    网站/笔记本基础设施所需 Python 依赖
LICENSE             代码的 MIT License
CONTENT-NOTICE.md   教育内容的 CC BY-SA 4.0 说明
```

## 本地使用

本项目目前还不是一个可在本地运行的完整课程。

现阶段的本地设置主要用于查看仓库源码和检查网站基础设施：

```bash
python -m pip install -r requirements.txt
quarto render
```

Quarto 需要单独安装。

## 笔记本

第 1 章笔记本文件目前是占位文件。等第一批实质课程内容写好后，再补充运行和复现说明。

## 贡献

本项目目前还没有进入一般性贡献阶段。

现阶段的改动应限于范围明确的基础设施、文档、翻译或审核任务。除非有专门 issue 明确范围，否则不应添加实质性行为经济学内容。

## 许可证

除非另有说明，教育内容使用 CC BY-SA 4.0 许可。见 `CONTENT-NOTICE.md`。

代码使用 MIT License。见 `LICENSE`。
