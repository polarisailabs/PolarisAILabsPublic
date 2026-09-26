# PolarisAI Labs

Public site for [polarisailabs.com](https://polarisailabs.com). Next.js builds it as a static website. Publish the generated `out/` directory.

## Requirements

- Node.js 20.9 or later
- npm

## Build

```bash
npm install
npm run build
```

`npm run build` writes the site to `out/`. That directory is the deployable site: HTML pages, `robots.txt`, `sitemap.xml`, images, and the `/_next` assets. `out/` is gitignored. Do not deploy `node_modules` or `.next`.

`npm run dev` runs the local development server at [http://localhost:3000](http://localhost:3000). `next start` does not serve this export.

Preview the static build locally:

```bash
npx serve out
```

## Deploy

Upload the **contents** of `out/` to the web root. 