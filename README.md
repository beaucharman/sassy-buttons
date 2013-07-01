# Sassy Buttons!

> Some clean styles and thoughtful Sass mixins that create sexy and semantic CSS button objects.

## Usage

1. Download and import `_sassy-buttons.scss` into your Sass directory.
2. Use the `sassy-button()` mixin to render the CSS necessary for each button style. For example:
```
@include sassy-button($label, $background-color, $foreground-color, $inverted, $high-contrast);
```
3. Make, and enjoy a pot of tea.

For more usage examples and demonstrations of the sassiness, [visit the project page](http://beaucharman.github.io/sassy-buttons).

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

### Button CSS object examples

The following `sassy-button()` mixin declarations are good starting points and are the example button CSS ojects on the [project page](http://beaucharman.github.io/sassy-buttons).

```scss
//
// Button object examples
//

// Primary button
@include sassy-button(primary, #6981c5, #fff);

// Danger button
@include sassy-button(danger, #d8544b, #fff);

// Success button
@include sassy-button(success, #7cbd55, #fff);

// Noir button
@include sassy-button(noir, #222, #fff);

// Custom coloured button
@include sassy-button(custom-color, #108a69, #fff);

// High contrast button
@include sassy-button(high-contrast, #f0af00, #fff, false, true);

// Inverted button
@include sassy-button(inverted, #a2c2f9, #000, true);
```