> **Please note:** This is an initial commit and is not yet ready for consumption. Please see the roadmap below. Please feel free to fork and contribute, but please be aware that usage may result in unexpected results.

# Sass Gradient Mixin

A simple Sass (SCSS) Gradient Mixin that provides the ability to quickly add Linear and Radial CSS3 Gradients.

## Roadmap

- Make `filter:` dynamic.
- Add `$reverse` option for radial gradients.
- Refactor and Refine coding.
- Add example use and github page.
- Complete further testing and establish appropriate browser stats.
- Complete usage documentation.
- Add sort order for color locations.
- Refine `@error` messages and `@warn` messages.
- Add appropriate comments to explain the code.

## Usage

The Sass Gradient Mixin accepts four variables. These are as follows:

```scss
sass-gradient($direction, $reverse, $colors, $fallback);
```

###$direction

**Type:** string

The '$direction' parameter dictates which direction/shape the gradient should display.

The following are accepted:

- `horizontal`: Gradients run from top to bottom (bottom to top in reverse).
- `vertical`: Gradients run from left to right (right to left in reverse).
- `diagonal-up`: Gradients run from bottom-left to top-right (top-right to bottom-left in reverse)
- `diagonal-down`: Gradients run from bottom-right to top-left (top-left to bottom-right in reverse)
- `radial`: Gradients run from center to outer (outer to center in reverse)

For more information and use cases please refer to the [Examples](#examples).

###$reverse

**Type:** boolean

The `$reverse` boolean can be set to reverse the colors in the map.

The following are accepted:

- `false`: Color's are displayed in the order represented in the `@map`.
- `true`: Color's are displayed in reverse order of the `@map`.

For more information and use cases please refer to the [Examples](#examples).

###$colors

**Type:** @map

Colors are applied via a Sass map. The key of the map is the percentage and the value is the color.

```scss
$sass-gradient-colors: (
	percentage: color
);
```

For more information and use cases please refer to the [Examples](#examples).

###fallback

**Type:** color

Fallback is a single color that is used for fallback in older browsers.

For more information and use cases please refer to the [Examples](#examples).

## Examples

Coming Soon.

## Resources

- [Colorzilla Gradient Creator](http://www.colorzilla.com/gradient-editor/) - The Sass Gradient Mixin was adapted from Colorzilla's CSS3 Gradient Creator.