# @e2agency/ea-fluid-adaptability

## Description

The `@e2agency/ea-fluid-adaptability` package provides a set of SCSS mixins and functions for easy handling of adaptive font and element size changes on a web page.

## Examples

- [CodePen](https://codepen.io/dowellkin/pen/MWxYNBa)

## Installation

Install the package using npm:

```bash
npm install @e2agency/ea-fluid-adaptability
```

## Usage

Import the package into your SCSS files:

```scss
@use "@e2agency/ea-fluid-adaptability" as *;
```

## Usage

Use the ea-rem and ea-rem-max functions for working with sizes in rem:

```scss
$my-size: ea-rem(20px); // Convert 20px to rem
$max-size: ea-rem-max(30px); // Convert 30px to rem and add the max() function
```

## Relative sizes

Use the ea-rel and ea-rel-max functions for working with relative sizes:

```scss
$rel-size: ea-rel(18px); // Size relative to the base size
$max-rel-size: ea-rel-max(25px); // Relative size with the addition of the max() function
```

## Clamp function

Use the ea-clamp function to create a CSS clamp function with adaptive sizes:

```scss
$adaptive-size: ea-clamp(10px, 30px, 500, 1000, "x"); // Create an adaptive size with clamp()
```

## API

See the [API documentation](API-documentation.md) for API of functions.

## License

MIT License

Copyright (c) 2023 Egorov Agency

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.