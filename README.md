# 函数之间 · 交互式微积分可视化

一个无需安装依赖的静态网页，用于探索常见函数、函数图像和微积分概念。

## 在线预览

直接在浏览器中打开 `index.html` 即可。

## 功能

- 提供多项式、三角、指数、对数、平方根、绝对值、反比例和有理函数模板。
- 支持修改 `a`、`b`、`c`、`d` 参数，或输入自己的函数表达式。
- 支持自定义 x 轴和 y 轴显示范围。
- 查看函数图像、数值导数、切线和定积分面积。
- 使用纯 HTML、CSS 和 JavaScript，无需安装依赖或运行构建步骤。

自定义表达式支持 `+`、`-`、`*`、`/`、`%`、`^`、括号，以及 `sin`、`cos`、`tan`、`sqrt`、`abs`、`ln`、`log`、`exp`、`min`、`max` 等函数。支持的写法和参数以页面中的表达式提示为准。导数和积分通过数值方法估算。

## 上传到 GitHub

### 使用 GitHub Desktop

1. 打开 GitHub Desktop，选择 **File → Add Local Repository**，选中本项目文件夹。
2. 填写提交说明，例如 `Create calculus visualization site`，然后选择 **Commit to main**。
3. 点击 **Publish repository**，登录 GitHub 并发布仓库。可按需选择公开或私有；如果希望别人能访问 Pages 网站，仓库需要允许 Pages 发布。

### 使用 Git 命令

在本项目文件夹内运行以下命令。初始化并提交后，可在 GitHub 新建空仓库，再把仓库地址替换为自己的地址：

```bash
git init
git add index.html README.md .github/workflows/pages.yml
git commit -m "Create calculus visualization site"
git branch -M main
git remote add origin https://github.com/你的用户名/function-calculus-visualizer.git
git push -u origin main
```

如果仓库已经初始化为 Git 仓库，可跳过 `git init`。如果远程仓库已经有提交，不要直接覆盖；先确认仓库内容并按需同步。

## 发布为 GitHub Pages 网站

项目已包含 GitHub Actions 自动部署配置。推送到 `main` 或 `master` 分支后会自动发布：

1. 在 GitHub 仓库打开 **Settings → Pages**。
2. 将 **Build and deployment → Source** 设置为 **GitHub Actions**。
3. 打开 **Actions** 标签，等待 **Deploy static site to GitHub Pages** 工作流完成。
4. 发布地址通常为 `https://你的用户名.github.io/仓库名/`。也可在 **Settings → Pages** 查看实际地址。

之后更新并推送 `index.html`，GitHub Actions 会再次发布网站。
