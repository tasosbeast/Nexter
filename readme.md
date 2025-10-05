# Nexter Starter

Nexter is a responsive landing page that spotlights premium real-estate listings. It pairs semantic HTML with modular Sass partials that compile into a single production stylesheet.

## Features

- CSS Grid layout spanning sidebar, hero, feature grid, listings, story, and gallery sections
- Shared Sass variables, spacing scale, and mixins to keep design tokens consistent
- Responsive breakpoints handled through a `respond()` mixin for size-specific tweaks
- Accessible focus outlines, keyboard-friendly controls, and scalable hover treatments ready for enhancement

## Prerequisites

- Node.js (version 16 or newer recommended)
- npm (bundled with Node.js)

## Install and Run

```bash
npm install           # install development dependencies
npm run start         # launch live-server and Sass watcher in parallel
```

The dev server hosts the project at http://127.0.0.1:8080 with automatic reload when files in `sass/` or `index.html` change.

## Build for Production

```bash
npm run build:css
```

This pipeline compiles Sass, runs Autoprefixer against the last 10 browser versions, and outputs a compressed `css/style.css`. Run it before committing or deploying.

## Deployment (GitHub Pages)

1. Execute `npm run build:css` to refresh the production CSS.
2. Commit `index.html`, `css/style.css`, and assets to a GitHub repository.
3. In **Settings -> Pages**, choose the `main` branch and the root (`/`) folder.
4. Save; GitHub Pages publishes to `https://<username>.github.io/<repo>/` within a few minutes.
5. Open the URL to confirm fonts, images, and responsive behaviour load correctly.

_Alternative:_ drag and drop the built folder into Netlify or Vercel for instant hosting and optional extras like redirects or form handling.

## Project Structure

```
starter/
|-- css/            # compiled stylesheets (style.css is the deployment target)
|-- img/            # image assets
|-- sass/           # Sass partials and main entry point
|-- index.html      # landing page markup
|-- package.json    # scripts and dev dependencies
`-- README.md
```

live-preview: https://tasosbeast.github.io/Nexter/
