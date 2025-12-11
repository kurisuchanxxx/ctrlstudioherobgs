# Dither Background

Full-screen dither effect background for Webflow iframe embedding.

## Development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Deploy to Vercel

1. Initialize git repository:
```bash
git init
git add .
git commit -m "init dither bg"
```

2. Create a new repository on GitHub and push:
```bash
git remote add origin https://github.com/YOUR_USERNAME/dither-bg.git
git branch -M main
git push -u origin main
```

3. Deploy on Vercel:
   - Go to https://vercel.com
   - Click "Add New Project"
   - Import your GitHub repository
   - Vercel will auto-detect Vite configuration
   - Click "Deploy"

## Webflow Integration

Use this iframe code in Webflow:

```html
<iframe
  src="https://YOUR-PROJECT.vercel.app"
  style="width: 100%; height: 100%; border: none;"
  loading="lazy"
></iframe>
```
