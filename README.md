# Toggl Track LinkedIn carousel — speculative portfolio concept

Independent concept; not an official publication or affiliated post.

## Deliverables

- `public/slides/slide-1.png` through `slide-4.png`: finished 1080 × 1350 artwork.
- `toggl-linkedin-carousel.pdf`: four-page PDF made from those exact artworks.
- `public/toggl-linkedin-carousel.pdf`: identical PDF served by the local site.
- Six application source files: `index.html`, `package.json`, `vite.config.js`, `src/main.jsx`, `src/App.jsx`, `src/style.css`.
- `carousel-source.pptx` and `build-slides.cjs`: optional editable/rendering sources.

## Run locally

Requires Node.js 20+ and an internet connection for initial npm package installation:

```bash
npm install
npm run dev
```

Open the local URL Vite prints. To build: `npm run build`. To preview: `npm run preview`.

## Deploy to Vercel

Import the folder/repository as a Vite project. The framework preset is Vite, build command `npm run build`, and output directory `dist`. Static files under `public/` are copied into the build.

## Notes about verification

The four exported slides were rendered and dimension-checked, and the four-page PDF was inspected for page count. The slides were validated with the slide overflow checker. The webpage's npm install/build could not be completed in the authoring environment because the package registry did not respond; run the commands above in an environment with npm registry access before deploying. No website deployment was performed.

The slide designs are original conceptual diagrams, not Toggl software screenshots; figures/proportions are illustrative. Toggl-inspired colors follow observed brand visual references; display type uses an available fallback rather than an unlicensed proprietary brand font. The word 'toggl' is set in text, not supplied as an official logo asset. Demo engagement data and fictional profiles are illustrative. The official CTA linked in the website was verified at https://toggl.com/blog/project-profits.


## Carousel image deployment fix
The four PNGs in `src/assets/` are imported directly into `src/App.jsx`, so Vite includes them in the production bundle. Commit the entire `src/assets/` directory to GitHub. The original files are also mirrored in `public/slides/` for easy inspection. The PDF is in `public/toggl-linkedin-carousel.pdf`. When uploading to GitHub manually, preserve folder names and paths: do not upload only the six code files.
