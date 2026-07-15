# 🗳️ PulseHub

<p align="left">
  <img src="https://img.shields.io/badge/Next.js-16-black" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-5-blue" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Tailwind-CSS-38bdf8" alt="Tailwind" />
  <img src="https://img.shields.io/badge/Prisma-ORM-2d3748" alt="Prisma" />
  <img src="https://img.shields.io/badge/SQLite-local-lightgrey" alt="SQLite" />
  <img src="https://img.shields.io/badge/shadcn%2Fui-components-000" alt="shadcn/ui" />
</p>

| Field | Value |
|-------|-------|
| **Title** | PulseHub |
| **Description** | A minimal local-first polling and voting app built with Next.js, TypeScript, Tailwind, shadcn/ui, and SQLite. |
| **Language** | TypeScript / Next.js App Router |
| **Tags** | `nextjs` · `typescript` · `tailwindcss` · `prisma` · `sqlite` · `shadcn-ui` · `polling` · `voting` |
| **Author** | Manya Chandra — [@Manyachandra](https://github.com/Manyachandra) |

**PulseHub** is a straightforward insight-capture tool: run polls, gather responses, and track choices in a clean interface. Instead of relying on external analytics or heavy survey platforms, it keeps everything in your own SQLite database with a front-end that feels immediate to use.

This repo includes:
- reactive UI with Next.js 16 App Router
- shadcn/ui-styled components for dialogs, tabs, selects, and notifications
- Prisma schema for polls, options, and votes
- local-first workflow with `npx prisma db push`

## Features

- 🚀 Next.js 16 App Router with TypeScript
- 🧩 shadcn/ui component patterns (`Button`, `Dialog`, `Select`, `Tabs`, `Sonner` toasts)
- 🗳️ Poll model with multiple options and vote tracking
- 💾 SQLite persistence through Prisma
- 🎨 Tailwind CSS v4 + CSS theme tokens
- 📱 Responsive layout

## Tech Stack

| Area | Choice |
|---|---|
| Framework | Next.js 16 |
| Language | TypeScript |
| Styling | Tailwind CSS v4 |
| Components | shadcn/ui |
| Database | SQLite via Prisma |
| Notifications | Sonner |
| Theme | next-themes |

## Project Structure

```
pulse-hub/
├── prisma/
│   ├── schema.prisma
│   └── prisma.config.ts
├── public/
├── src/
│   ├── app/
│   │   ├── globals.css
│   │   ├── layout.tsx
│   │   └── page.tsx
│   ├── components/ui/
│   │   ├── badge.tsx
│   │   ├── button.tsx
│   │   ├── card.tsx
│   │   ├── dialog.tsx
│   │   ├── dropdown-menu.tsx
│   │   ├── input.tsx
│   │   ├── label.tsx
│   │   ├── select.tsx
│   │   ├── sonner.tsx
│   │   ├── tabs.tsx
│   │   └── textarea.tsx
│   └── lib/
│       └── utils.ts
├── components.json
├── .env
├── .gitignore
├── eslint.config.mjs
├── next.config.ts
├── package.json
└── tsconfig.json
```

## Getting Started

```bash
# install dependencies
npm install

# prepare prisma client and local DB
npx prisma db push
npx prisma generate

# start dev server
npm run dev
```

Open `http://localhost:3000`.

## Database

Schema lives in `prisma/schema.prisma`.

```bash
npx prisma db push
npx prisma generate
```

## Author

**Manya Chandra**
- GitHub: https://github.com/Manyachandra
- Email: manyachandra@proton.me
