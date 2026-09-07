# 个人主页（academicpages 结构）

一个基于 [academicpages](https://academicpages.github.io) 模板结构重建的 Jekyll 个人主页，内容为李宗睿的博士研究生主页。

## 📁 目录结构

```
.
├── _config.yml              # 站点与作者信息
├── _data/
│   └── navigation.yml       # 顶部导航菜单
├── _pages/                  # 页面（关于 / 发表论文 / CV / 404）
│   ├── about.md             # 首页
│   ├── publications.md      # 论文列表
│   └── cv.md                # 简历
├── _publications/           # 每篇论文一个 Markdown 文件
├── _bibliography/
│   └── papers.bib           # BibTeX 引用
├── _layouts/                # 页面布局
├── _includes/               # 顶栏 / 侧边栏 / 页脚等组件
├── assets/                  # CSS / JS
├── images/                  # 头像等图片
└── Gemfile                  # Ruby 依赖
```

## 🚀 本地预览（需要 Ruby + Jekyll）

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve
```

然后访问 http://localhost:4000

> 本机若未安装 Ruby，可先安装 [RubyInstaller](https://rubyinstaller.org/)（Windows）。

## 🌐 部署到 GitHub Pages

1. 新建仓库 `Zongrui-Li.github.io`，把本项目文件推送到 `main` 分支。
2. 在 `_config.yml` 中设置 `url: "https://zongrui-li.github.io"`。
3. GitHub Pages 会自动用 Jekyll 构建发布。

## ✏️ 待补充内容

| 位置 | 说明 |
| --- | --- |
| `_publications/2026-title-tbd.md` | 论文 2606.03495 的标题与作者 |
| `images/profile.svg` | 替换为你的真实头像（`images/profile.png` 等） |
| `_config.yml` 的 `url` / `repository` | 填你的 GitHub Pages 地址 |
