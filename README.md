# 🚧 Work in Progress
Updating this repo when I have time. Feel free to contribute! 🫡

## To-Do List V 1.0.0
- [x] PNpm Monorepo
- [x] Next.js
- [x] Nest.js
- [x] Global Typescript Config
- [ ] tRPC
- [ ] Linting
- [ ] Tailwind
- [ ] Shadcn.UI
- [ ] Drizzle ORM || Prisma
- [ ] Jest || Vitest
- [ ] Storybook
- [ ] Cypress
- [ ] Husky
- [ ] Vercel
- [ ] Docker
- [ ] CI/CD
- [ ] Versioning
- [ ] Documentation

## To-Do List V 2.0.0
- [ ] Expo-React Native
- [ ] E2E Testing
- [ ] CLI
- [ ] Templates

<br><br><br>

## ⚠️ Disclaimer
- I'm not claiming to be an expert, just a developer who is learning and sharing my knowledge with others.
- This is just one way of doing things. It may not be the best or the worst, but it's one approach to consider.
- Technology is simply a tool. Choose the right tool for the job at hand.
- I cannot be held responsible for any damage that may result from using this repository. Please use it at your own risk.

<br><br><br>

# ⚡️ Full-Stack Type-Safe PNpm Monorepo with Next.js 13.4+ App Router, NestJS & tRPC

- This monorepo is fully end-to-end type safe.
- The tRPC server is fully integrated into NestJS, giving you access to all of its powerful features such as dependency injection.
- It's a great fit for the transition to server-side rendering in Next.js 13.
- The frontend(s) and backend projects are kept separate, but they work together seamlessly within the monorepo.

### Why PNpm instead of Yarn or NPM workspaces?
- If you're unsure about using a monorepo, it may not be the best choice for you. Maintaining a monorepo can be a lot of work, and it may not be worth it unless you have a large project.

### Why PNpm Monorepo instead of Nx or Turborepo?
- Both Turborepo and Nx are great tools, but they can be a bit too opinionated. I wanted to keep the monorepo as simple as possible and be able to use the NestJS CLI to generate new modules, controllers, services, etc. without having to worry about the file structure imposed by Nx or Turborepo.
- If your project grows to the point where Nx or Turborepo would be beneficial, it's easy to migrate to one of those tools later on.

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
