# Work in progress

* Updating files: 100% (1/3), done.

---

# ⚡️ Full-Stack Type-Safe PNpm Monorepo with Next.js 13.4+ App Router, NestJS & tRPC

- It's fully end-to-end type safe
- The tRPC server is fully integrated into NestJS, so you have access to all of NestJS's wonderful functionality like dependency injection
- Fits really well with the Next.js 13 transition to server side rendering
- It keeps the frontend(s) and backend project separate, but seamlessly working together in the monorepo

## Pre-Requisites

- [pnpm](https://pnpm.io/installation)
- [NestJS CLI](https://docs.nestjs.com/cli/overview)

## Run:

First make sure you add an `.env.local` file inside the `web` app with the following variable:

```env
NEXT_PUBLIC_NESTJS_SERVER=http://localhost:4000
```

Then run:

```
pnpm install
pnpm dev       # starts local server for both frontend (NextJS) and backend (NestJS)
```
