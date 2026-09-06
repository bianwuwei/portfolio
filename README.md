# 吴小为 · Wei Wu 个人作品集

基于 Astro + TypeScript 的静态个人作品集 / 产品站，路径前缀 /portfolio/。

预览：https://bianwuwei.github.io/portfolio/

## 包含内容

- Hero：姓名与产品人定位
- 关于我：简短中文介绍
- 精选作品：3 个占位项目
- 能力与关注：产品设计、路线规划、交付落地
- 联系方式：GitHub + 邮箱占位

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

产物在 dist/。astro.config.mjs 已设置 site 与 base: /portfolio/。

## 技术栈

Astro 7 + TypeScript；纯静态。中文界面。

## 发布

静态产物已提交到 docs/，可将 GitHub Pages 来源设为 main 分支的 /docs。
重新构建后请同步更新 docs/：bun --bun run build && rm -rf docs && cp -a dist docs && touch docs/.nojekyll
