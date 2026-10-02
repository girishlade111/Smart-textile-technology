# WRLDS — Smart Textile Technology

A marketing website for **WRLDS**, a smart-textile technology company embedding sensors and electronics into fabrics. Showcases project case studies (FireCat, sport retail, workwear, hockey, pet tracker), technology details, development process, blog, careers, and company info — built with React, Vite, TypeScript, shadcn/ui and Tailwind CSS.

## Features

- Landing page with hero, stats, and product highlights
- Project case-study pages: FireCat, Sport Retail, Workwear, Hockey, Pet Tracker
- Tech Details and Development Process pages
- Blog with article detail pages
- About, Careers, Privacy Policy pages
- Custom 404 page
- Dark/light theme toggle (next-themes)
- Toast notifications (shadcn/ui Sonner), charts (Recharts), animations (Framer Motion)
- Cookie banner, OG image, sitemap.xml, robots.txt

## Tech Stack

- React 18 + TypeScript
- Vite (build)
- React Router v6
- shadcn/ui (Radix primitives) + Tailwind CSS
- TanStack React Query
- Framer Motion, Recharts, react-hook-form

## Quick Start

```bash
git clone https://github.com/girishlade111/Smart-textile-technology.git
cd Smart-textile-technology
npm install --legacy-peer-deps
npm run dev        # dev server at http://localhost:8080
```

## Build

```bash
npm run build      # outputs static site to dist/
npm run preview    # preview the production build
```

## Project Structure

```
Smart-textile-technology/
├── index.html              # Entry HTML (title: WRLDS)
├── vite.config.ts          # Vite config (base path for GitHub Pages)
├── src/
│   ├── App.tsx             # Router + providers (basename: /Smart-textile-technology)
│   ├── main.tsx            # Entry point
│   ├── pages/              # Index, project pages, TechDetails, Blog, About, Careers, …
│   ├── components/         # shadcn/ui components + custom sections
│   ├── data/               # Content data
│   ├── hooks/              # Custom hooks
│   └── lib/                # Utilities
├── public/                 # favicon, og-image, sitemap.xml, robots.txt, uploads
└── tailwind.config.ts      # Tailwind config
```

## Env Vars

None required. (Contact form uses `emailjs-com` — wire your own EmailJS keys in the contact component if you re-enable it.)

## Deploy Notes

Static export. Served via GitHub Pages from the `gh-pages` branch (built `dist/` output): https://girishlade111.github.io/Smart-textile-technology/

To redeploy: run `npm run build`, copy `dist/` contents to a `gh-pages` branch, and push. The Vite `base` and React Router `basename` are both set to `/Smart-textile-technology` so assets and routes resolve under the Pages subpath; a `404.html` copy of `index.html` handles deep-link refreshes.

---

Built by [Girish Lade](https://github.com/girishlade111) · [ladestack.in](https://ladestack.in)
