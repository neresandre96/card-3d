# Card3D

> Beautiful 3D card

[![NPM](https://img.shields.io/npm/v/card-3d.svg)](https://www.npmjs.com/package/3d-flip-card) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save 3d-flip-card
```

## Usage

```tsx
import React, { Component } from 'react'

import MyComponent from '3d-flip-card'
import '3d-flip-card/card-styles.css'

class Example extends Component {
  render() {
    return 
    <Card3D
      height="300px"
      width="200px"
      thickness={10}
      rotationSpeed={10}
      hoverToStop={true}
      mode="clickToFlip"
      leftColor="green"
      rightColor="yellow"
    >
      <div>Frente do Cartão</div>
      <div>Verso do Cartão</div>
    </Card3D>
  }
}
```

## Demo

[Demo](https://neresandre96.github.io/card-3d/)

## Props

The Card component has the following customizable props:

| Prop            | Type                                   | Description                                                                                      |
|-----------------|----------------------------------------|--------------------------------------------------------------------------------------------------|
| `children`      | `ReactNode[]`                         | The child elements of the card; must contain exactly two elements.                             |
| `height`        | `string`                              | The height of the card (can use units like '100px', '50%', etc.).                             |
| `width`         | `string`                              | The width of the card (can use units like '100px', '50%', etc.).                             |
| `thickness`     | `number`                              | The thickness of the card in pixels.                                                           |
| `rotationSpeed` | `number`                              | The rotation speed of the card in degrees per second. Default is 0.                            |
| `hoverToStop`   | `boolean`                             | Determines if the rotation should stop when hovering over the card. Default is false.          |
| `mode`          | `"dragToFlip" | "clickToFlip"`      | The interaction mode for flipping the card.                                                    |
| `leftColor`     | `string`                              | The color of the left side of the card.                                                        |
| `rightColor`    | `string`                              | The color of the right side of the card.                                                       |

## Documentation

The Card component is a React component that renders a 3D card with customizable properties. It uses CSS3D transformations to create a 3D effect.
To see full documentation, visit [documentation](https://neresandre96.github.io/card-3d/).

## Observations

The component expects exactly two children. Otherwise, a warning will be displayed in the console and the card will not be rendered.
The properties rotationSpeed and hoverToStop have default values that can be changed as needed.

## Contributing
Feel free to contribute with improvements and corrections! Open a pull request or create an issue to discuss your ideas.

## License

MIT © [neresandre96](https://github.com/neresandre96)
