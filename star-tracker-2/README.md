# Homework Star Tracker (Netlify deploy)

## Project setup

```bash
cd /Users/pranaysethi/Documents/GitHub/rbl_hw/star-tracker-2
npm install
```

## Run locally

```bash
npm run dev
```

## Build for production

```bash
npm run build
```

## Netlify Deployment (recommended)

1. Sign in to Netlify and connect your GitHub repository to this project.
2. In Site settings, set:
   - Build command: `npm run build`
   - Publish directory: `dist`
3. Add branch deploy trigger for `main`.
4. Add `netlify.toml` (already added).

### Alternative command line deploy

```bash
npm i -g netlify-cli
npm run build
netlify deploy --prod --dir=dist
```

## Notes

- `netlify.toml` includes a fallback redirect for SPA routing.
- The app code lives in `src/HomeworkStarTrackerApp.jsx`.
