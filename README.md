# DailyScrum powered by Turborepo

## What's inside?

This repo uses [pnpm](https://pnpm.io) as a packages manager. It includes the following packages/apps:

### Apps and Packages

- `frontend`: a [ReactJS](https://reactjs.org) app
- `backend`: [Fastify X Typescript](https://fastify.io) app
- `ui`: a stub React component library shared by both `frontend` and `backend` applications
- `config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `tsconfig`: `tsconfig.json`s used throughout the monorepo

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### Utilities

This turborepo has some additional tools already setup for you:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Prettier](https://prettier.io) for code formatting

## Setup

This repository is used in the `npx create-turbo@latest` command, and selected when choosing which package manager you wish to use with your monorepo (PNPM).

Further packages to install globally:
```
npm i -g pnpm commitizen create-turbo@latest
```

### Build

To build all apps and packages, run the following command:

```
git clone git@github.com:sagarrkhanal/DailyScrum.git
cd DailyScrum
pnpm install

```

### Develop & Running

To develop all apps and packages, run the following command:

```
pnpm run dev
```

### Commit Style:
```bash
git commit -m "feat(api): AB#5 add feature message here"
```

### Feature Development
<font color='green'>Each task/pbi/bug must have its own branch with ID prefix in the name.
Always create new branch from dev.</font>

Eg.:
```bash
git checkout -b "AB#5/projectSetup"
```

### Task/Bug Lifecycle
 * PBI/Bugs will be in "To Do" state
 * When you start working on it - move it to "In Progress"
 * When you are done with work and need to create PR - do so and then move task to "Review"
 * When the PR is merged - this will be automatically moved to "Done"

### DOD (Definition of Done)
- PR must be reviewed and approved 
- Completely done feature, completely done bugs
- Must handle errors
- No Console.log
- No debugger
- Must pass unit test and 70% coverage
- No Lint erros
- Clean Code with appropriate formatting
- Use as much as possible ES6
- Action/Status must pass

## Useful Links

Learn more about the power of Turborepo:

- [Pipelines](https://turborepo.org/docs/features/pipelines)
- [Caching](https://turborepo.org/docs/features/caching)
- [Remote Caching (Beta)](https://turborepo.org/docs/features/remote-caching)
- [Scoped Tasks](https://turborepo.org/docs/features/scopes)
- [Configuration Options](https://turborepo.org/docs/reference/configuration)
- [CLI Usage](https://turborepo.org/docs/reference/command-line-reference)
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/#specification)
- [Husky,Commitizen](https://folafunmi.hashnode.dev/a-guide-to-order-setting-up-prettier-and-eslint-with-husky-lint-staged-and-commitizen)
