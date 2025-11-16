# panel_codex

## Fixing the missing `autoprefixer` dependency

If you see Vite crash with an error similar to:

```
Failed to load PostCSS Plugin failed: Cannot find module 'autoprefixer'
```

it means the project does not have the [`autoprefixer`](https://github.com/postcss/autoprefixer) package installed. Install it as a dev dependency and restart the dev server:

```bash
npm install --save-dev autoprefixer
npm run dev
```

This makes the `postcss.config.js` file load correctly and lets Vite continue serving the application.