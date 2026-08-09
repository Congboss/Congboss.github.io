# 我的博客

基于 [Astro](https://astro.build/) 的个人博客，主题使用 [AstroPaper](https://github.com/satnaing/astro-paper)，部署在 GitHub Pages 上。

## 写一篇新文章

1. 在 `src/content/posts/` 下新建一个 `.md` 文件（文件名建议用英文短横线，比如 `my-first-post.md`）；
2. 在文件开头写好 frontmatter，参考 [hello-world.md](src/content/posts/hello-world.md)：

   ```md
   ---
   author: qiancong
   pubDatetime: 2026-08-09T12:00:00+08:00
   title: "文章标题"
   draft: false
   tags:
     - 技术
   description: "文章的一句话简介。"
   ---
   ```

3. 正文直接写 Markdown 即可，代码块、标题、图片、表格都能正常渲染；
4. 提交并推送：

   ```bash
   git add .
   git commit -m "新文章：xxx"
   git push
   ```

推送后 GitHub Actions 会自动构建并发布，等一两分钟就能在线上看到。

## 本地预览

```bash
pnpm install
pnpm run dev
```

然后打开 http://localhost:4321 。

## 常用命令

- `pnpm run dev`：本地开发预览
- `pnpm run build`：构建静态站点（输出到 `dist/`）
- `pnpm run preview`：本地预览构建结果

## 致谢

主题来自 [AstroPaper](https://github.com/satnaing/astro-paper)，感谢作者的优秀工作。
