# Stars

`<Stars />` is a component that renders stars in the sky of your scene. It is an abstraction that use Points, PointsMaterial, and BufferGeometry to create a beautiful starry effect.

<!-- <StackBlitzEmbed projectId="tresjs-text3d-cientos" /> -->

## Usage

You can use the `<Stars />` component without passing any props, but you can use props from the table below to tweak the settings to better suit your needs.

```vue
<template>
  <TresCanvas>
  ...
    <Stars />
    ...
  </TresCanvas>
</template>
```

Notice that you can pass a texture as an alphaMap to modify the star shape.

```vue
<template>
  <TresCanvas>
  ...
    <Stars :radius="50" :depth="20" :count="3000" :alphaMap="alphaMap"  />
    ...
  </TresCanvas>
</template>
```
## Props

| Prop               | Description                                                            | Default |
| :----------------- | :--------------------------------------------------------------------- | ------- |
| **size**           | The size of the stars.                        |   0.1      |
| **sizeAttenuation**           | Keep the same size regardless distance.|   true      |
| **transparent**           | Show transparency on the stars texture.                                 | true     |
| **alphaTest**         | Enables WebGL to know when not to render the pixeltext.                                                | 0.01     |
| **alphaMap**  | Texture of the stars. | null      |
| **count**   | Number of stars.      | 5000    |
| **depth** | Depth of the stars' shapes.                         | 50    |
| **radius**      | Radius of the stars' shapes.                            | 100    |
| **factor**    | Star scale randomness factor.                           | 4       |
