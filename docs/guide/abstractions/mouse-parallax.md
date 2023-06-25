# MouseParallax

![](/cientos/MouseParallax.gif)

`<MouseParallax />` is a component that allows you to easily create the pam parallax effect. The camera will update automatically according to the mouse position, creating a beautiful, nice effect.

## Usage

You only need import it to use it. Additionally, you can pass two props: ease and factor.

`factor` is a number to modify the movement range of the camera. `ease` is a boolean that toggles smooth transitions. In addition, you can disable with the `disabled` prop.

```vue
<template>
  <TresCanvas>
    <MouseParallax />
    <Text3D text="TresJS" font="/fonts/FiraCodeRegular.json">
      <TresMeshNormalMaterial />
    </Text3D>
  </TresCanvas>
</template>
```

## Props

| Prop         | Description                                             | Default |
| :----------- | :------------------------------------------------------ | ------- |
| **disabled** | enable or disabled the effect, boolean                  | false   |
| **factor**   | Modify the range of the parallax                        | 2.5     |
| **ease**     | enable or disabled the easing effect                    | true    |
