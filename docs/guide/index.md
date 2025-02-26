# Cientos

![Cientos banner](/cientos-banner.png)

> Cientos (Spanish word for "hundreds", pronounced `/θjentos/` ) is a collection of useful, ready-to-go helpers and components that are not part of the [core](/guide/index.md) package. The name uses the word uses in spanish to multiply by 100, to refer to the potential reach of the package to hold a amazing abstractions.

The `cientos` package uses the [`three-stdlib`](https://github.com/pmndrs/three-stdlib) module under the hood instead of `three/examples/jsm`. This means that you don't need to extend the catalogue of components using the `extend` method; `cientos` does it for you.

It just works. 💯

::: info
This package is not required to use the core library, but it can make your developer experience much better, especially for complex scenes.
:::

## Installation

::: code-group

```bash [pnpm]
pnpm add @tresjs/cientos
```

```bash [npm]
npm install @tresjs/cientos

```

```bash [yarn]
yarn add @tresjs/cientos
```

:::

## Basic Usage

```ts
import { OrbitControls } from '@tresjs/cientos'
```

Now you can use the `OrbitControls` component in your scene.

```html
<template>
  <TresCanvas shadows alpha>
    <TresPerspectiveCamera :args="[45, 1, 0.1, 1000]" />
    <OrbitControls />
  </TresCanvas>
</template>
```

::: warning
Notice that you don't need to write the prefix `Tres` such as `<TresOrbitControl />` to use the component
:::
