# InsightsIQ Landing (Vite + React + Tailwind)

A ready-to-deploy marketing site for **insightsIQ.us**.

## 1) Preview locally (optional)
1. Install Node.js (LTS).
2. In a terminal:
   ```bash
   npm install
   npm run dev
   ```
   Open the printed localhost URL.

## 2) Deploy — Vercel (easiest)
1. Push this folder to GitHub.
2. Go to https://vercel.com → **New Project** → Import your repo.
3. Framework: **Vite**; Build: `npm run build`; Output: `dist/`.
4. After deploy, open **Settings → Domains** and add `insightsIQ.us`.
5. At your domain registrar, create:
   - A record `@` → `76.76.21.21`
   - CNAME `www` → `cname.vercel-dns.com`
6. Back in Vercel → **Verify** (SSL will auto-enable).

### Contact form (Formspree)
- Sign in at https://formspree.io, create a form and copy its endpoint ID.
- In `src/App.jsx`, replace `YOUR_ENDPOINT` in the `<form action="...">` with your ID.

## 3) Deploy — Netlify (also easy)
1. New site from Git → select this repo.
2. Build: `npm run build` ; Publish: `dist/`.
3. **Domains** → add `insightsIQ.us`. Follow DNS instructions.
4. To use **Netlify Forms**, comment out the Formspree form and uncomment the Netlify form in `src/App.jsx`.

## 4) Customize
- Text, sections, and links live in `src/App.jsx` near the top (arrays: `features`, `steps`, `products`, `integrations`).

---
© 2025 InsightsIQ. All rights reserved.
