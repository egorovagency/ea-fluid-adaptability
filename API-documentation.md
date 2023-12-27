# @e2agency/ea-fluid-adaptability API Documentation

## Functions

### `ea-unit($value)`

Converts a value to pixels.

### `ea-rem($size, $base-size: $ea-base-size)`

Converts a size to `rem` based on a specified base size.

### `ea-rem-max($size, $base-size: $ea-base-size, $min-size: $ea-min-size)`

Generates a `max()` function for a size in `rem` based on a specified base size and minimum size.

### `ea-rel($size, $base-size-variable: "--ea-font-size")`

Generates a `calc()` function for a size relative to a specified base size variable.

### `ea-rel-max($size, $base-size-variable: "--ea-font-size", $min-size: $ea-min-size)`

Generates a `max()` function for a size relative to a specified base size variable and minimum size.

### `ea-view-units($axis)`

Returns the appropriate viewport units ("vw" for X-axis, "vh" for Y-axis).

### `ea-clamp($min-size, $max-size, $min-resolution, $max-resolution, $axis: "x")`

Generates a `clamp()` function with adaptive sizes based on minimum and maximum sizes, minimum and maximum resolutions, and an optional axis.

## Usage

See the [README](README.md) for examples of how to use these functions in your SCSS files.

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
