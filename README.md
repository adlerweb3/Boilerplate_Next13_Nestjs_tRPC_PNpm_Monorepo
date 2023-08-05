# 🚧 Work in Progress
Updating this repo when I have time. Feel free to contribute! 🫡

## To-Do List

- [x] PNpm Monorepo
- [x] Next.js
- [x] NestJS
- [x] Global Typescript Config
- [_] tRPC
- [ ] Linting
- [ ] Tailwind
- [ ] Shadcn.UI
- [ ] Drizzle ORM
- [ ] Jest
- [ ] Storybook
- [ ] Cypress
- [ ] Husky
- [ ] Vercel
- [ ] Docker
- [ ] CI/CD
- [ ] Versioning
- [ ] Documentation

<br><br><br>

# ⚡️ Full-Stack Type-Safe PNpm Monorepo with Next.js 13.4+ App Router, NestJS & tRPC

- It's fully end-to-end type safe
- The tRPC server is fully integrated into NestJS, so you have access to all of NestJS's wonderful functionality like dependency injection
- Fits really well with the Next.js 13 transition to server side rendering
- It keeps the frontend(s) and backend project separate, but seamlessly working together in the monorepo

# Why PNpm Monorepo instead of Nx or Turborepo?
- Turborepo and Nx are great, but they are a bit too opinionated. I wanted to keep the monorepo as simple as possible, and I wanted to be able to use the NestJS CLI to generate new modules, controllers, services, etc. without having to worry about Nx or Turborepo's file structure.
- Once the project is in production and larger to the point where Nx or Turborepo would be beneficial, it's easy to migrate to them.

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
