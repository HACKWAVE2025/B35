# VidhiSahayak Web

Professional legal assistant website built with Next.js (App Router), TypeScript, Tailwind CSS, and shadcn/ui.

## Features

- Home: hero, search, featured categories, support CTA
- Categories: list and detail pages with guidance placeholders
- Consultation: lawyers listing placeholder
- Dashboard: user and lawyer areas (placeholders)
- AI Chat: `/chat` with `/api/chat` placeholder endpoint
- File-based data for categories (Vercel-ready, no DB required)

## Getting Started (Local)

Install dependencies and start dev server:

```bash
npm install
npm run dev
```

Open http://localhost:3000

## Production Build

```bash
npm run build
npm start
```

## Deploy on Vercel

1. Push this folder to a GitHub repository (e.g. `vidhisahayak-web`).
2. Go to https://vercel.com/new and import the repo.
3. Framework Preset: Next.js (auto-detected). No extra env vars needed for this version.
4. Deploy.

Optional next steps (will require env vars if added):
- Supabase (DB + Auth)
- Stripe (payments)
- OpenAI/LLM key for AI chat

## Project Structure

- `src/app` — routes (App Router)
- `src/components` — UI components (Navbar, Footer)
- `src/lib/categories.ts` — file-based categories
- `src/app/api/chat/route.ts` — placeholder chat API

## Roadmap

- Auth and roles (user/lawyer/consultant) with onboarding
- Real database (Supabase) for categories, lawyers, consultations
- Payments for bookings
- AI chat integration with retrieval
