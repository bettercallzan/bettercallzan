<p align="center">
  <img src="public/logos/better-call-saul-logo.png" alt="Better Call Saul Logo" width="320" />
</p>

<h1 align="center">Better Call Saul — Legal Consulting Landing Page</h1>

<p align="center">
  A bold, premium landing page template for legal consulting services.<br/>
  Built with <strong>Next.js 15</strong>, <strong>Tailwind CSS v4</strong>, and <strong>Framer Motion</strong>.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-15-black?logo=next.js" alt="Next.js" />
  <img src="https://img.shields.io/badge/React-19-61DAFB?logo=react" alt="React" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?logo=tailwindcss" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/Framer_Motion-12-FF0055?logo=framer" alt="Framer Motion" />
  <img src="https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript" alt="TypeScript" />
</p>

---

## 📋 Overview

**Better Call Saul** is a modern, fully responsive landing page template designed for law firms, legal consultants, and professional services. Inspired by the iconic *Better Call Saul* TV series aesthetic, it combines a bold visual identity with a premium user experience.

This template is **production-ready** and can be easily customized with your own brand identity, content, and imagery.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🎨 **Premium Design** | Bold gradients, gold accents, and a dark/red color scheme that feels professional and authoritative |
| 📱 **Fully Responsive** | Pixel-perfect layouts from mobile (320px) to ultrawide desktop screens |
| 🎬 **Smooth Animations** | Scroll-triggered animations with Framer Motion for a premium feel |
| 📝 **Multi-Step Form** | Interactive consultation booking flow with package selection, legal area, case details, and contact info |
| 💬 **WhatsApp Integration** | One-click WhatsApp consultation button for direct client communication |
| 🎠 **Touch Carousels** | Swipeable carousels for services, packages, and testimonials on mobile |
| 🧩 **Modular Sections** | 12 independent, reusable section components for easy customization |
| ⚡ **Blazing Fast** | Built on Next.js 15 App Router with optimized images and font loading |
| ♿ **Accessible** | Radix UI primitives ensure proper accessibility out of the box |

---

## 🏗️ Project Structure

```
bettercallsaul/
├── app/
│   ├── components/           # Shared app components
│   │   ├── motion-wrapper.tsx    # Framer Motion animation wrappers
│   │   ├── scroll-to-top.tsx     # Scroll-to-top floating button
│   │   └── section-header.tsx    # Reusable section title component
│   ├── sections/             # Page sections (each self-contained)
│   │   ├── navbar/               # Fixed navigation bar
│   │   ├── hero/                 # Hero banner with CTA
│   │   ├── about/                # About / profile section
│   │   ├── services/             # Legal areas bento grid
│   │   ├── packages/             # Pricing packages
│   │   ├── process/              # Multi-step consultation form
│   │   ├── configurator/         # Alternative form configurator
│   │   ├── testimonials/         # Client testimonials carousel
│   │   ├── faq/                  # Frequently asked questions
│   │   ├── contact/              # Contact CTA section
│   │   └── footer/               # Footer with links & info
│   ├── globals.css           # Global styles & design tokens
│   ├── layout.tsx            # Root layout with fonts
│   └── page.tsx              # Main page assembling all sections
├── components/
│   └── ui/                   # shadcn/ui base components
│       ├── accordion.tsx
│       ├── button.tsx
│       ├── card.tsx
│       ├── checkbox.tsx
│       ├── input.tsx
│       ├── label.tsx
│       ├── radio-group.tsx
│       ├── select.tsx
│       └── textarea.tsx
├── lib/
│   └── utils.ts              # Utility functions (cn helper)
└── public/
    ├── images/               # All image assets
    │   ├── testimonials/         # Testimonial profile images
    │   └── ...                   # Hero, service, contact backgrounds
    └── logos/                # Brand logos
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** 18.17 or later
- **npm**, **yarn**, **pnpm**, or **bun**

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/rinkira26/bettercallsaul.git

# 2. Navigate to the project
cd bettercallsaul

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.

### Build for Production

```bash
npm run build
npm start
```

---

## 🎨 Customization Guide

### Changing Brand Colors

Edit the CSS custom properties in `app/globals.css`:

```css
:root {
  --navy: oklch(0.25 0.05 250);       /* Primary dark color */
  --navy-dark: oklch(0.15 0.04 250);  /* Darker variant */
  --gold: oklch(0.75 0.15 85);        /* Accent / CTA color */
  --gold-light: oklch(0.85 0.12 85);  /* Light accent variant */
}
```

### Replacing Images

Simply replace the files in the `public/images/` directory:

| File | Used In | Recommended Size |
|------|---------|-----------------|
| `heros.jpg` | Hero background | 1920×1080px |
| `who-is-saul.webp` | About section | 800×800px (square) |
| `service-saul.jpg` | Services background | 800×1200px |
| `saul-contact.jpg` | Contact background | 1920×1080px |
| `saul-packages.png` | FAQ decoration | 400×400px (transparent PNG) |
| `testimonials/*.jpg` | Testimonial cards | 400×500px |

### Updating Content

All section content (text, links, data) is defined directly inside each section component in `app/sections/[section-name]/index.tsx`. Simply edit the arrays and strings to match your business.

---

## 🌐 Deployment

### Option 1: Vercel (Recommended)

The easiest and fastest way to deploy — optimized for Next.js out of the box.

1. Push your code to a GitHub repository
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub
3. Click **"Add New Project"**
4. Select your `bettercallsaul` repository
5. Vercel will auto-detect it as a Next.js project
6. Click **"Deploy"** — that's it! 🎉

> Your site will be live at `https://your-project.vercel.app` within ~60 seconds.

### Option 2: Netlify

1. Push your code to GitHub
2. Go to [netlify.com](https://netlify.com) and sign in
3. Click **"Add new site"** → **"Import an existing project"**
4. Connect your GitHub repository
5. Set the build settings:
   - **Build command:** `npm run build`
   - **Publish directory:** `.next`
6. Click **"Deploy site"**

> **Note:** Install the [Next.js Netlify plugin](https://docs.netlify.com/frameworks/next-js/overview/) for full compatibility.

### Option 3: Railway

1. Go to [railway.app](https://railway.app) and sign in with GitHub
2. Click **"New Project"** → **"Deploy from GitHub repo"**
3. Select your repository
4. Railway auto-detects Node.js and runs `npm run build && npm start`
5. Your site will be assigned a public URL automatically

### Option 4: Docker (Self-Hosted)

Create a `Dockerfile` in the project root:

```dockerfile
FROM node:18-alpine AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

FROM node:18-alpine AS runner
WORKDIR /app
COPY --from=builder /app/.next ./.next
COPY --from=builder /app/public ./public
COPY --from=builder /app/package*.json ./
COPY --from=builder /app/node_modules ./node_modules
EXPOSE 3000
CMD ["npm", "start"]
```

Then build and run:

```bash
docker build -t bettercallsaul .
docker run -p 3000:3000 bettercallsaul
```

### Option 5: Static Export (Any Hosting)

If you don't need server-side features, you can export as a static site:

1. Add to `next.config.ts`:
   ```ts
   const nextConfig = { output: 'export' };
   ```
2. Run:
   ```bash
   npm run build
   ```
3. Upload the `out/` folder to any static hosting (GitHub Pages, Firebase Hosting, AWS S3, etc.)

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| [Next.js 15](https://nextjs.org/) | React framework with App Router |
| [React 19](https://react.dev/) | UI library |
| [Tailwind CSS v4](https://tailwindcss.com/) | Utility-first CSS |
| [Framer Motion](https://www.framer.com/motion/) | Scroll & entrance animations |
| [Radix UI](https://www.radix-ui.com/) | Accessible UI primitives |
| [Lucide React](https://lucide.dev/) | Icon library |
| [React Icons](https://react-icons.github.io/) | Additional icons (WhatsApp, etc.) |
| [TypeScript](https://www.typescriptlang.org/) | Type safety |

---

## 📄 License & Disclaimer

> **PORTFOLIO DISCLAIMER:** This website is a creative portfolio project designed for demonstration purposes only. It is not an actual legal service or official site. "Better Call Saul", its characters, and related media are the intellectual property of **AMC Network Entertainment LLC** and **Sony Pictures Television Inc.** All rights belong to their respective owners.

---

<p align="center">
  Made with ❤️ and a little bit of legal trouble.
</p>
