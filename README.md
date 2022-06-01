# vue3-vite-class-component

Project template using Vue3 with Vite and vue-class-component

## Setup

Used `npm init vue@lastest` as recommanded on the Quick start page of Vue.js.

Cleared the default files to leave only one `HelloWorld` component.

Added `vue-class-component` using `npm install --save vue-class-component@8.0.0-rc.1`

## Problem

VSCode displays an error on `Vue` in `HelloWorld.vue` :

```
Type 'typeof import(".../vue3-vite-class-component/node_modules/vue-class-component/dist/vue-class-component")' is not a constructor function type. ts(2507)
```

Running `npm run build`, I get the following error:

```
'default' is not exported by node_modules/vue-class-component/dist/vue-class-component.esm-bundler.js, imported by src/components/HelloWorld.vue
file: .../vue3-vite-class-component/src/components/HelloWorld.vue:1:7
1: import Vue from "vue-class-component";
          ^
2: export class HomePage extends Vue {
3:   constructor() {
error during build:
Error: 'default' is not exported by node_modules/vue-class-component/dist/vue-class-component.esm-bundler.js, imported by src/components/HelloWorld.vue
```