# cmdr.blog

A personal blog and portfolio built with [Astro](https://astro.build), styled with [Tailwind CSS](https://tailwindcss.com) and the [Everforest Soft](https://github.com/sainnhe/everforest) color scheme.

## Stack

- **Astro** - Static site generator
- **Tailwind CSS 4** - Utility-first CSS with `@tailwindcss/typography` for prose
- **Everforest Soft** - Adaptive light/dark color scheme
- **GitHub API** - Projects fetched from GitHub at build time

## Structure

```
src/
  components/    Astro components (Header, Footer, Search, Breadcrumbs)
  content/blog/  Blog posts in Markdown/MDX
  layouts/       Shared page layout
  pages/         Routes (posts, projects, 404)
  styles/        Global CSS with Everforest variables
public/          Static assets (favicon, robots.txt)
```

## Commands

| Command           | Action                               |
| :---------------- | :----------------------------------- |
| `npm install`     | Install dependencies                 |
| `npm run dev`     | Start dev server at `localhost:4321` |
| `npm run build`   | Type-check and build to `./dist/`    |
| `npm run check`   | Run Astro type checker               |
| `npm run preview` | Preview build locally                |
