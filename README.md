# @e2agency/ea-fluid-adaptability

## Description

The `@e2agency/ea-fluid-adaptability` package provides a set of SCSS mixins and functions for easy handling of adaptive font and element size changes on a web page.

## Docs

You can find the full and detailed documentation [here](https://egorovagency.notion.site/ea-fluid-adaptability-en-030062c7043647d2af6afca3cd9a1eb3).

## Examples

- Basic usage
  - [CodePen](https://codepen.io/dowellkin/pen/MWxYNBa)
  - [StackBlitz](https://stackblitz.com/edit/js-xguxsw?file=scss%2Fdemo.scss)

## Installation

Install the package using npm:

```bash
npm install @e2agency/ea-fluid-adaptability
```

## Usage

1. Import the package into your SCSS files:

```scss
@use "@e2agency/ea-fluid-adaptability" as *;
```
2. Set `font-size` to html using `ea-clamp()`:

```scss
html {
  font-size: ea-clamp(10, 16, 1200, 1920); // clamp(10px, 0px + 0.8333333333vw, 16px)
}
```

2. Define container size using `ea-clamp()`:

```scss
.container {
  max-width: ea-clamp(320, 1680, 360, 1920); // clamp(320px, 6.1538461538px + 87.1794871795vw, 1680px)
}
```

4. Use the `ea-rem` and `ea-rem-max` functions for working with sizes in rem:

```scss
body {
  font-size: ea-rem-max(16); // max(1rem, 14px)
}

.section {
  padding: ea-rem(80) 0; // 5rem 0
}
```

## Relative sizes

Define css-variable `--ea-font-size` using `ea-clamp()` and use the `ea-rem` and `ea-rem-max` functions for working with relative sizes:

```scss
:root {
  --ea-font-size: #{ea-clamp(10.7, 16, 1280, 1920)}; // clamp(10.7px, 0.1px + 0.828125vw, 16px)
}

body {
  font-size: ea-rel-max(16); // max(calc(16 * var(--ea-font-size, 16px) / 16), 14px)
}

.section {
  padding: ea-rel(80) 0; // calc(80 * var(--ea-font-size, 16px) / 16) 0
}
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