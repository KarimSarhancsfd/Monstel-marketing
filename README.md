# MONSTEL | Strategic Growth & Regional Expansion Plan

Interactive digital presentation for MONSTEL Hair Care.

---

## 🚀 Deployment on Vercel

This repository is optimized for deployment on **Vercel**.

### Option A: Automatic GitHub Integration (Recommended)

1. Ensure changes are pushed to GitHub:
   ```bash
   git add .
   git commit -m "Add Vercel DevOps configuration"
   git push origin master
   ```
2. Go to your [Vercel Dashboard](https://vercel.com/dashboard).
3. Click **"Add New..."** → **"Project"**.
4. Import the `Monstel-marketing` repository.
5. Keep default framework settings (Framework Preset: **Other** / Static Site).
6. Click **Deploy**.

Vercel will automatically build, deploy, and assign a production URL with SSL/TLS and global CDN caching.

---

### Option B: Deploying via Vercel CLI

1. Install Vercel CLI globally:
   ```bash
   npm i -g vercel
   ```
2. Run deployment from the project directory:
   ```bash
   vercel
   ```
3. To deploy to production:
   ```bash
   vercel --prod
   ```

---

## ⚙ DevOps & Optimization Features (`vercel.json`)

- **Edge CDN Frame Caching**: `background-frames/*` images are served with `Cache-Control: public, max-age=31536000, immutable` for maximum rendering performance.
- **Security Headers**: Includes `X-Content-Type-Options`, `X-Frame-Options`, `X-XSS-Protection`, and `Referrer-Policy`.
- **Clean URLs**: Clean URL routing enabled (`cleanUrls: true`).
- **CI Workflow**: Included `.github/workflows/vercel-ci.yml` validates configuration integrity on every push.

---

## 🛠 Local Development

To run the presentation locally:

```bash
npx serve .
```

Then open `http://localhost:3000` in your browser.
