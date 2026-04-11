# Note Reviewer — Landing Page

Official marketing website for the **Note Reviewer** Chrome Extension — an AI-powered quality and compliance tool for
BCBAs working in Applied Behavior Analysis (ABA).

Built with [Astro](https://astro.build) + [Tailwind CSS](https://tailwindcss.com).  
A product by **Infinity Code LLC** · [info@notereviewer.org](mailto:info@notereviewer.org)

---

## 🚀 Project Structure

```text
/
├── public/
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   ├── assets/
│   ├── components/
│   │   └── Welcome.astro
│   ├── layouts/
│   │   └── Layout.astro          # Shared HTML shell (head, fonts, meta)
│   ├── pages/
│   │   ├── index.astro           # Landing page (Hero, Features, How it Works, Privacy & Trust, CTA, Footer)
│   │   └── privacy.astro         # Full Privacy Policy page
│   └── styles/
│       └── global.css
└── package.json
```

---

## 🛠️ Local Development

### Prerequisites

- [Node.js](https://nodejs.org/) ≥ 18
- [pnpm](https://pnpm.io/) ≥ 8

### Install dependencies

```sh
pnpm install
```

### Start dev server

```sh
pnpm dev
```

The site will be available at `http://localhost:4321`.

---

## 📦 Build for Production

```sh
pnpm build
```

The optimized static output is generated in the `dist/` folder.

To preview the production build locally:

```sh
pnpm preview
```

---

## 🌐 Deployment

This site is a fully static Astro project and can be deployed to any static hosting provider.

### Netlify (recommended)

1. Connect your repository to [Netlify](https://netlify.com).
2. Set the **Build command** to `pnpm build`.
3. Set the **Publish directory** to `dist`.
4. Deploy. Netlify will automatically handle routing for the `/privacy` page.

### Vercel

1. Import the repository on [Vercel](https://vercel.com).
2. Vercel auto-detects Astro — no extra configuration needed.
3. Click **Deploy**.

### GitHub Pages

Add an `astro.config.mjs` `base` and `site` option if deploying to a subpath, then push to the `gh-pages` branch or use
the official [Astro GitHub Pages GitHub Action](https://docs.astro.build/en/guides/deploy/github/).

---

## 📄 Privacy Policy

The Privacy Policy for the Note Reviewer Chrome Extension is located at:

```
src/pages/privacy.astro
```

**Live URL:** `https://your-domain.com/privacy`

This page covers:

- What data is processed (clinical note text for real-time AI analysis).
- Confirmation that **no PHI is stored** on Infinity Code LLC servers.
- Data encryption in transit via HTTPS/TLS to the API at `infinitycodellc.com`.
- Commitment to **never sell or share** user data with third parties for advertising.
- HIPAA considerations and guidance for clinicians.
- User rights and contact information.

To update the "Last updated" date, edit the `lastUpdated` variable at the top of `src/pages/privacy.astro`.

---

## 📬 Contact & Support

| Channel  | Details                                               |
|----------|-------------------------------------------------------|
| Email    | [info@notereviewer.org](mailto:info@notereviewer.org) |
| WhatsApp | [+1 786-644-7422](https://wa.me/17866447422)          |
| Company  | Infinity Code LLC                                     |

---

## 📝 License

© 2025 Infinity Code LLC. All rights reserved.
