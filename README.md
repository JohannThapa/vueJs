# Vue.js project

This template should help get you started developing with Vue 3 in Vite.

# Creating a Vue Application

```sh
 npm init vue@latest
```

This command will install and execute create-vue, the official Vue project scaffolding tool. You will be presented with prompts for several optional features such as TypeScript and testing support:

```sh
✔ Project name: … <vureJs>
✔ Add TypeScript? … No / Yes ==> Yes
✔ Add JSX Support? … No / Yes ==> Yes
✔ Add Vue Router for Single Page Application development? … No / Yes ==> Yes
✔ Add Pinia for state management? … No / Yes ==> Yes
✔ Add Vitest for Unit testing? … No / Yes ==> Yes
✔ Add Cypress for both Unit and End-to-End testing? … No / Yes ==> Yes
✔ Add ESLint for code quality? … No / Yes ==> Yes
✔ Add Prettier for code formatting? … No / Yes ==> Yes
```

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin) to make the TypeScript language service aware of `.vue` types.

If the standalone TypeScript plugin doesn't feel fast enough to you, Volar has also implemented a [Take Over Mode](https://github.com/johnsoncodehk/volar/discussions/471#discussioncomment-1361669) that is more performant. You can enable it by the following steps:

1. Disable the built-in TypeScript Extension
    1) Run `Extensions: Show Built-in Extensions` from VSCode's command palette
    2) Find `TypeScript and JavaScript Language Features`, right click and select `Disable (Workspace)`
2. Reload the VSCode window by running `Developer: Reload Window` from the command palette.

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
npm run test:unit
```

### Run End-to-End Tests with [Cypress](https://www.cypress.io/)

```sh
npm run test:e2e:dev
```

This runs the end-to-end tests against the Vite development server.
It is much faster than the production build.

But it's still recommended to test the production build with `test:e2e` before deploying (e.g. in CI environments):

```sh
npm run build
npm run test:e2e
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
# Project structure

    .
    ├── ...
    ├── cypress               # Front end testing tool
    │   ├── e2e                 # E2E Test (End-to-end)
    │   ├── fixtures            # Json file
    │   └── support             # Support file (commands etc)
    ├── public                # Static files
    ├── src                   # Main source files
    │   ├── assets               # Other assets file like images, styles etc.
    │   ├── components           # Vue components
    │   │    ├── __tests__         # Test files (alternatively `spec` or `tests`)
    │   │    └── icons             # Icons
    │   ├── router               # Vue routing
    │   ├── stores               # Vue stores (State Management)
    │   └── views                # UI components
    ├── .eslintrc             # esLint config file  
    ├── .prettierrc           # Prettier config file 
    ├── .cypress.config       # Cypress config file     
    ├── .index.html           # Main file because of SPA 
    ├── .package.json         # JSON file for configuration of packages.     
    ├── .tsconfig             # Typescript config file  
    └── .vite.config          # Config file (build tool)to set up a development environment.