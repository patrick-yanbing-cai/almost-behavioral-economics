# Almost Behavioral Economics

Almost Behavioral Economics 是一个中英双语的行为经济学开源学习项目。Project Yuki 保留为内部代号。

本仓库当前只包含基础设施：Quarto 网站骨架、中英文页面结构、第 1 章占位笔记本、共享参考文献文件，以及最小 Python 包结构。

## 网站

GitHub Pages 地址：仓库发布后配置。

语言入口：

- `zh/`
- `en/`

## 当前状态

基础设施骨架已初始化。实质性经济学内容尚未编写。

## 仓库结构

```text
zh/                 中文网站页面和笔记本
en/                 英文网站页面和笔记本
src/yuki/           最小 Python helper package 骨架
references.bib      共享 BibTeX 参考文献
_quarto.yml         Quarto 网站配置
```

## 本地设置

安装 Python 依赖：

```bash
python -m pip install -r requirements.txt
```

Quarto 需要通过官方发行版单独安装。

## 构建网站

```bash
quarto render
```

本地预览：

```bash
quarto preview
```

## 运行笔记本

可在 Jupyter 中打开 `zh/notebooks/` 或 `en/notebooks/` 下的笔记本：

```bash
jupyter notebook
```

## 贡献

请保持改动聚焦。基础设施、正文内容、翻译和审核工作应尽量分开处理。

## 许可证

除非另有说明，本仓库中的教育内容使用 CC BY-SA 4.0 许可。见 `LICENSE-CONTENT.md`。

本仓库中的代码使用 MIT License。见 `LICENSE`。
