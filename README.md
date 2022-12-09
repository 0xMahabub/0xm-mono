# Mono repository with yarn workspace

## Used Techs :=>

> A simple mono-repository using `yarn` workspace.

```yml
name: A simple mono-repository
workspace: yarn-workspace
node:
  working_version: node:18.x
  engines:
    # for vite it must be >=14.18.x
    node: >=18.x
    npm:  >=8.x
package-manager: yarn@1.22.19
```

```yml
# create frontend apps quickly
react:
  js-app: `yarn g:vite --template react`
  ts-app: `yarn g:vite --template react-ts`

vue:
  js-app: `yarn g:vite --template vue`
  ts-app: `yarn g:vite --template vue-ts`

svelte:
  js-app: `yarn g:vite --template svelte`
  ts-app: `yarn g:vite --template svelte-ts`

ssg-astro:
  docs: `yarn g:docs`

angular: `yarn g:ng`

```
