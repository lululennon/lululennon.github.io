# lululennon.github.io

个人主页 + 技术博客，部署于 GitHub Pages。纯 HTML/CSS/JS，零依赖、零构建。

## 本地预览

```bash
# 任选其一，在项目根目录执行
python3 -m http.server 8000
# 然后浏览器打开 http://localhost:8000
```

## 如何发布一篇新文章

1. 复制 `posts/hello-world.html`，重命名为如 `posts/my-note.html`
2. 修改 `<title>`、文章标题、日期和正文
3. 在 `index.html` 的 `post-grid` 里复制一个卡片块，把 `href` 指向新文章，更新标题、摘要、日期和 tag

## 目录结构

```
├── index.html          # 首页（Hero + 文章列表 + 关于）
├── css/style.css       # 全部样式（深色主题，含变量定义，改颜色在 :root）
├── js/main.js          # 滚动渐现动画
└── posts/              # 文章页
    └── hello-world.html
```

## 自定义

- **配色**：`css/style.css` 顶部的 `:root` 变量（`--accent`、`--gradient` 等）
- **头像**：`index.html` 中 `about-avatar`，可换成 `<img>`
- **链接**：导航和关于区的 GitHub / Email 链接改成自己的

## 部署

推送到 `main` 分支即可，GitHub Pages 自动发布（Settings → Pages → Source: main / root）。
