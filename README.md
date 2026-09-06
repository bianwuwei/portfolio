# 無為 · Wu Wei 个人站点

基于 Astro + TypeScript 的个人开发者 / builder 站点，路径前缀 `/portfolio/`。

预览：https://bianwuwei.github.io/portfolio/

GitHub：[@bianwuwei](https://github.com/bianwuwei)

## 包含内容

- Hero：無為 / Wu Wei，独立交付个人产品与开源
- 关于：重新出发、公开学习；轻量提及过往 AI 相关经验（无公司名）
- 产品与开源：本站 + 即将公开的个人项目占位
- 能力：构建交付、产品感觉、AI 实验、开放协作
- 联系：`luwuwei328@gmail.com` + GitHub

## 本地开发

需要 Node.js >= 22.12（也可用 Bun）。

```bash
npm install
npm run dev
```

默认地址：http://localhost:4321/portfolio/

## 构建与预览

```bash
npm run build
npm run preview
```

产物在 `dist/`。`astro.config.mjs` 已设置 `site` 与 `base: /portfolio/`。

## 技术栈

Astro 7 + TypeScript；纯静态。中文为主界面，兼顾国际读者。

## 发布

静态产物提交到 `docs/`，GitHub Pages 来源为 `main` 分支的 `/docs`。

重新构建后请同步更新 docs：

```bash
bun --bun run build && rm -rf docs && cp -a dist docs && touch docs/.nojekyll
```
