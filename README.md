# Mall Dashboard

Vite + React app, ready to deploy to Vercel.

## Local development

```bash
npm install
npm run dev
```

Then open http://localhost:5173.

## Production build

```bash
npm run build      # outputs to ./dist
npm run preview    # preview the production build locally
```

## Deploy to Vercel

**Option A — GitHub + Vercel dashboard (easiest):**

1. Push this folder to a GitHub repo.
2. Go to https://vercel.com/new and import the repo.
3. Vercel auto-detects Vite. Defaults are correct:
   - Framework Preset: **Vite**
   - Build Command: `npm run build`
   - Output Directory: `dist`
4. Click **Deploy**.

**Option B — Vercel CLI:**

```bash
npm install -g vercel
vercel        # follow prompts; accept defaults
vercel --prod # promote to production
```

The included `vercel.json` rewrites all routes to `/` so client-side routing works if you add it later.
