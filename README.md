# 📚 Research Notes

基于 [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) 的科研笔记站点。

## 🚀 快速开始

### 1. 本地预览

```bash
# 安装依赖
pip install -r requirements.txt

# 启动本地服务器（支持热重载）
mkdocs serve
```

浏览器打开 `http://127.0.0.1:8000` 即可实时预览。

### 2. 部署到 GitHub Pages

推送到 `main` 分支即可自动部署（通过 GitHub Actions）。

```bash
git add .
git commit -m "add: 新笔记"
git push
```

## 📁 目录结构

```
research-notes/
├── mkdocs.yml              # 站点配置（导航、主题、插件）
├── requirements.txt        # Python 依赖
├── docs/
│   ├── index.md            # 首页
│   ├── javascripts/
│   │   └── mathjax.js      # LaTeX 公式配置
│   ├── notes/              # 知识点笔记
│   ├── papers/             # 论文阅读笔记
│   └── blog/               # 博客文章
└── .github/workflows/
    └── deploy.yml          # 自动部署工作流
```

## ✏️ 写新笔记

1. 在 `docs/notes/` 或 `docs/papers/` 下新建 `.md` 文件
2. 在 `mkdocs.yml` 的 `nav` 部分添加对应条目
3. 提交推送，自动部署

## 📐 LaTeX 公式

- 行内公式：`\( E = mc^2 \)`
- 独立公式块：
```
\[
\nabla \cdot \mathbf{E} = \frac{\rho}{\varepsilon_0}
\]
```
