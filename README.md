<div align="center">
  <img src="public/favicon.svg" alt="E2E HRC Logo" width="80" />
  <h1 align="center">E2E HRC — Workforce Solutions</h1>
  <p align="center">
    Corporate website for E2E Human Resource Consultancy, a UK-based recruitment and workforce solutions firm.
  </p>
</div>

<p align="center">
  <a href="https://github.com/rahulchaudhari31/workforce-solutions/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License"></a>
  <img src="https://img.shields.io/github/repo-size/rahulchaudhari31/workforce-solutions" alt="Repo Size">
</p>

## Overview

E2E HRC provides permanent recruitment, contract staffing, executive search, international recruitment, RPO, and workforce consultancy services. This website serves as a marketing landing page showcasing the company's services, process, client testimonials, FAQs, and contact information.

## Tech Stack

| Technology   | Purpose                         |
| ------------ | ------------------------------- |
| React 19     | UI framework                    |
| Vite 8       | Build tool / dev server         |
| Tailwind CSS 3 | Utility-first CSS framework   |
| PostCSS      | CSS processing                  |
| react-icons  | Icon library (Feather icons)    |
| Oxlint       | Linter                          |
| Vercel       | Deployment                      |

## Getting Started

```bash
cd e2e-hrc
npm install
npm run dev
```

Build for production:

```bash
npm run build
npm run preview
```

## Project Structure

```
e2e-hrc/
├── public/                  # Static assets (favicon, SVG sprites)
├── src/
│   ├── assets/              # Images (hero.png, etc.)
│   ├── components/          # React components
│   │   ├── Navbar.jsx       # Sticky nav with mobile hamburger
│   │   ├── Hero.jsx         # Hero section with stats
│   │   ├── Solutions.jsx    # 6 service cards
│   │   ├── HowWeWork.jsx    # 6-step process
│   │   ├── Testimonials.jsx # Client testimonials
│   │   ├── FAQAndCTA.jsx    # FAQ accordion + CTA card
│   │   └── Footer.jsx       # Footer with contact info
│   ├── hooks/
│   │   └── useScrollReveal.js # IntersectionObserver animations
│   ├── App.jsx              # Root component
│   ├── main.jsx             # Entry point
│   └── index.css            # Tailwind + custom styles
├── index.html               # HTML entry
├── vite.config.js           # Vite configuration
├── tailwind.config.js       # Tailwind theme (colors, fonts)
├── postcss.config.js        # PostCSS plugins
├── vercel.json              # Vercel deployment config
└── package.json             # Dependencies & scripts
```

## Customization

### Colors & Fonts

Edit `tailwind.config.js`:

- **Primary:** `#0F2A52` (deep navy)
- **Accent:** `#F5A623` (gold/amber)
- **Background:** `#F2EFEA` (warm gray)
- **Text:** `#5A6472` (muted gray)
- **Headings:** Poppins / Sora
- **Body:** Inter / Poppins

### Animations

The `useScrollReveal` hook triggers fade-in/translate-up animations as sections enter the viewport. Customize offset and duration in `src/hooks/useScrollReveal.js`.

### Services

To add or modify service offerings, edit the `services` array in `src/components/Solutions.jsx`.

## Deployment

The project is pre-configured for **Vercel** via `vercel.json`. The root is set to `e2e-hrc/` with build command `npm run build` and output directory `dist`.

```bash
npm run build
npx vercel --prod
```

## Attribution

- Hero image placeholder from [Unsplash](https://unsplash.com)
- Icons from [Feather Icons](https://feathericons.com) via `react-icons`
- Fonts: [Poppins](https://fonts.google.com/specimen/Poppins), [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts

## License

[MIT](LICENSE)
