# Vishwa homepage

Complete static homepage with editable HTML, CSS and JavaScript, an original WebGL opening, policy animations, and individual image assets. No dependency installation or backend is required.

## Run locally

Use Node.js 18 or newer:

```sh
npm run build
npm start
```

Open http://127.0.0.1:4187. Set `PORT` to use another port.

## Source and deployment

- `partials/`: the page shell and editable sections, styles and interaction code.
- `public/`: original animation code, locally hosted fonts and separate image/logo assets.
- `scripts/build.mjs`: portable, dependency-free static build.
- `dist/`: complete deployable output. Serve this directory at the domain root.

`npm run build` writes production metadata for `https://vishwalab.com/` and permits indexing. `npm run build:preview` defaults to `http://127.0.0.1:4187/` and disables indexing. Set the `SITE_URL` environment variable before building to use a different canonical domain; both the canonical link and Open Graph URL use that value.

Navigation and product links continue to their existing external destinations. This project supplies the homepage; it does not recreate the banking application, CLI, vault, or other linked products.

## Editing

Edit the corresponding file in `partials/`, then rebuild. The build uses only files in this repository. Images, logos, the Inter font and the original Three.js renderer are stored locally in `public/`; no image is a screenshot of the whole page. The opening animation and trust transition retain their original renderer and timing. Reduced-motion visitors receive a static or manual presentation.

GPU cards link to published provider pricing. Displayed locations describe publicly documented service regions, not live inventory. Pricing and location evidence are recorded in `docs/`.

GitHub delivery excludes account-specific hosting configuration, credentials, local QA captures and intermediate archives.
