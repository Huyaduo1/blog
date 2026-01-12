# BlogWeb

一个基于 Hugo 的极简个人站点，包含简历式首页与博客列表页。

## 技术栈

- Hugo（静态站点生成器）
- 自定义模板：`layouts/`
- 自定义样式：`assets/css/custom.css`

## 目录结构

- `content/` 页面与文章内容
- `layouts/` Hugo 模板
- `assets/` Hugo Pipes 处理的资源（CSS）
- `res/` 静态资源（图片等）

## 本地开发

```bash
hugo server -D
```

然后打开终端输出的本地地址。

## 部署

已配置 GitHub Actions 自动部署到 GitHub Pages，推送到 `main` 即可自动构建与发布。

## 备注

- 若修改 GitHub Pages 路径，请同步更新 `hugo.toml` 的 `baseURL`。
- 静态资源来自 `static/` 与 `res/` 两个目录。
