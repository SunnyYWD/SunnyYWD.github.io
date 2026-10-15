# Wenda Yu · Personal Website

An English academic portfolio adapted from [PRISM](https://github.com/xyjoey/PRISM) (upstream commit `f2748db9821e98ed487eee5104ce4cc282aa8c1e`). The original MIT license and attribution are retained.

## Local development

Requires Node.js 22 or later.

```sh
npm ci
npm run dev
```

Open <http://localhost:3000/>.

## Edit the website

- Profile, navigation, and site settings: `content/config.toml`
- Biography: `content/bio.md`
- Experience: `content/experience.md`
- News: `content/news.toml`
- Papers and descriptions: `content/publications.bib`; figures: `public/papers/`
- Academic service and interview: `content/service.toml`
- Projects and links: `content/projects.toml`
- Portrait: `public/profile-photo.jpg`

The homepage contains About, Experience, News, Publications, and Service. Projects have a separate page.

## Build and deploy

`npm run build` exports the site to `out/`. Pushing to `main` triggers the GitHub Pages workflow in `.github/workflows/deploy.yml`. Set the repository's Pages source to **GitHub Actions**. The site URL is <https://sunnyywd.github.io/>.
