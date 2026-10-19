# Tyler Ronning's personal site

A Vue 3 and Tailwind CSS starter deployed to GitHub Pages with Vite.

## Run locally

Requires Node.js 20.19+ and npm.

```sh
npm ci
npm run dev
```

Vite prints a local URL. Open it in a browser to work on the site. To create and preview a production build:

```sh
npm run build
npm run preview
```

## Make it yours

- Edit the homepage, about copy, and project cards in `src/App.vue`.
- Update the page title and description in `index.html`.
- Change colors, typography, and other global styles in `src/style.css`.
- Replace the example email address and project links with your own.

## Publish to GitHub Pages

The workflow in `.github/workflows/deploy.yml` builds and deploys the site whenever a commit reaches `main`.

In the repository on GitHub, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**. After that, push to `main`; the Pages workflow will publish the `dist` build. The repository includes a `package-lock.json`; the workflow installs the exact locked versions with `npm ci`.
