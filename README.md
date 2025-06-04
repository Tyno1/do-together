# Do Together – Instant Activity-Based Friendships

**Do Together** is a next-generation social fitness network designed to help people connect through real-world **shared activities**, not endless chats. Users match based on activity and availability, meet up, and then decide — within **24 hours** — whether to become friends. It's friendship by doing, not talking.

---

## 🔥 What Makes Do Together Different?

> **No swiping. No ghosting. Just meet, move, and decide.**

- **Activity-First, Not Chat-First**: Skip awkward intros. Join someone for a hike, gym session, or walk.
- **The 24-Hour Friendship Window**: After the meetup, users must decide to connect — or let it go.
- **Intent-Driven Matching**: You know exactly what the other person wants to do and when.
- **Momentum Over Messaging**: No pen-pal phase. You go from discovery → meet-up → decision in one day.

---

## 🚀 Features

- 🔍 **Instant Matching** – Based on activity, time, location, and intent  
- 📅 **24-Hour Decision Window** – Encourages genuine evaluation, not connection hoarding  
- ✅ **Real-Time Attendance Check-In** – Confirmed meetups only  
- 🎯 **Streaks & Accountability** – Build consistency with others  
- 🧑‍🤝‍🧑 **1-on-1 & Group Modes** – Squad up or go solo  
- 🧭 **Discovery Tools** – Try new experiences with new people  

---

## 🧱 Tech Stack

| Layer        | Tech                             |
|--------------|----------------------------------|
| Frontend     | Next.js 14 (App Router)          |
| Styling      | Tailwind CSS + shadcn/ui         |
| Backend      | Node.js (Planned), Prisma ORM    |
| Auth         | NextAuth.js with JWT + Cookies   |
| Database     | PostgreSQL (via Prisma)          |
| Deployment   | Vercel / Railway (TBD)           |

---

| Phase      | Goal                                   |
| ---------- | -------------------------------------- |
| ✅ Phase 1  | MVP: Matching + Meetups + 24h window   |
| 🔜 Phase 2 | Social feed, streaks, groups           |
| 🔄 Phase 3 | Launch iOS/Android via Expo            |
| 🔐 Phase 4 | AI-based suggestions & retention tools |


## 📁 Monorepo Structure (Turborepo)



## Project Setup

This project uses Turborepo for monorepo management. Below is the documentation for the setup:

# Turborepo Setup Details

This Turborepo includes the following packages/apps:

### Apps and Packages

- `docs`: a [Next.js](https://nextjs.org/) app
- `web`: another [Next.js](https://nextjs.org/) app with shadcn/ui components
- `@repo/ui`: a stub React component library shared by both `web` and `docs` applications
- `@repo/eslint-config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `@repo/typescript-config`: `tsconfig.json`s used throughout the monorepo

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### Utilities

This Turborepo has some additional tools already setup for you:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Prettier](https://prettier.io) for code formatting

### Build

To build all apps and packages, run the following command:

```
cd my-turborepo
pnpm build
```

### Develop

To develop all apps and packages, run the following command:

```
cd my-turborepo
pnpm dev
```

### Remote Caching

Turborepo can use a technique known as [Remote Caching](https://turborepo.com/docs/core-concepts/remote-caching) to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can [create one](https://vercel.com/signup?utm_source=turborepo-examples), then enter the following commands:

```
cd my-turborepo
npx turbo login
```

This will authenticate the Turborepo CLI with your [Vercel account](https://vercel.com/docs/concepts/personal-accounts/overview).

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

```
npx turbo link
```

## Useful Links

Learn more about the power of Turborepo:

- [Tasks](https://turborepo.com/docs/crafting-your-repository/running-tasks)
- [Caching](https://turborepo.com/docs/crafting-your-repository/caching)
- [Remote Caching](https://turborepo.com/docs/core-concepts/remote-caching)
- [Filtering](https://turborepo.com/docs/crafting-your-repository/running-tasks#using-filters)
- [Configuration Options](https://turborepo.com/docs/reference/configuration)
- [CLI Usage](https://turborepo.com/docs/reference/command-line-reference)
