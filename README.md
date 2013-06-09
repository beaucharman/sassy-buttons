# Sassy Buttons!

> Some styles and functions to help quickly create nice buttons, with Sass ;)

## Usage

1. Download and import `_sassy-buttons.scss` into your Sass directory.
2. Use the `sassy-button()` mixin function to render the CSS necessary for each button style. For example:
```css
@include sassy-button($label, $background-color, $foreground-color, $inverted, $high-contrast);
```
3. Make, and enjoy a pot of tea.

### Mixin parameter descriptions

**$label**

The CSS selector that will be created (appended to btn--).

**$background-color**

The background color of the button, also used for gradients and borders.

**$foreground-color**

Used for text color and highlights.

**$inverted**

Awesome for aiding with the illusion of light source, alternating the placement of the text-shadow for dark text on light backgrounds (rather than the default light text on dark backgrounds - not inverted)

**$high-contrast**

Toggle the foreground and background colors on hover for high contrast user feedback.