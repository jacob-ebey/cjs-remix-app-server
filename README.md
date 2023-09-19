# Welcome to Remix!

This repo exists as an example of what it takes to use CJS instead of ESM in remix V2. Essentially, if your existing app is CJS, add `serverModuleFormat: "cjs"` to your `remix.config.js`. Here is the full diff as of 2.0.0 [https://github.com/jacob-ebey/cjs-remix-app-server/commit/de2b18b4c04c8b4c6f7205300e13df4b38699a79](https://github.com/jacob-ebey/cjs-remix-app-server/commit/de2b18b4c04c8b4c6f7205300e13df4b38699a79)

There is currently a bug where `--manual` doesn't bust the CJS module cache.

- [Remix Docs](https://remix.run/docs)

## Development

From your terminal:

```sh
npm run dev
```

This starts your app in development mode, rebuilding assets on file changes.

## Deployment

First, build your app for production:

```sh
npm run build
```

Then run the app in production mode:

```sh
npm start
```

Now you'll need to pick a host to deploy it to.

### DIY

If you're familiar with deploying node applications, the built-in Remix app server is production-ready.

Make sure to deploy the output of `remix build`

- `build/`
- `public/build/`
