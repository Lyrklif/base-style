
# CSS Utility Classes and Functions

This documentation provides an overview of various utility classes and functions for styling text, buttons, borders, and more in your frontend project.

## Table of Contents
1. [Text Utility Classes](#text-utility-classes)
  - [Text Color](#text-color)
  - [Text Font Family](#text-font-family)
  - [Text Weight](#text-weight)
  - [Text Alignment](#text-alignment)
  - [Text Decoration](#text-decoration)
  - [Text Transformation](#text-transformation)
  - [Text Size](#text-size)
  - [Line Height](#line-height)
2. [Margin and Padding Utility Classes](#margin-and-padding-utility-classes)
  - [Margin Auto](#margin-auto)
  - [Directional Margin and Padding](#directional-margin-and-padding)
3. [Layout Width Utility Classes](#layout-width-utility-classes)
4. [Display, Align Items, and Justify Content](#display-align-items-and-justify-content)
5. [Cursor Utility Classes](#cursor-utility-classes)
6. [Border and Rounded Utility Classes](#border-and-rounded-utility-classes)
7. [Background Color Utility Classes](#background-color-utility-classes)
8. [Button Utility Classes](#button-utility-classes)
9. [Fill Utility Classes](#fill-utility-classes)
10. [CSS Functions](#css-functions)
  - [`em()` function](#em-function)
  - [`rem()` function](#rem-function)

---

## Text Utility Classes

### Text Color
Use the `.text-color-[variant]` class to apply different text colors.

**Template**: `<p class="text-color-blue">text</p>`

Available variants:
- `.text-color-[variant]`: Apply the specific color to text.

### Text Font Family
Use the `.text-ff-[variant]` class to set the font family.

**Template**: `<p class="text-ff-secondary">text</p>`

Available variants:
- `.text-ff-primary`
- `.text-ff-secondary`

### Text Weight
Use the `.text-weight-[variant]` class to set the font weight.

**Template**: `<p class="text-weight-bold">text</p>`

Available variants:
- `.text-weight-regular`
- `.text-weight-medium`
- `.text-weight-semibold`
- `.text-weight-bold`

### Text Alignment
Use the `.text-align-[variant]` class to align text.

**Template**: `<p class="text-align-center">text</p>`

Available variants:
- `.text-align-left`
- `.text-align-center`
- `.text-align-right`
- `.text-align-justify`
- `.text-align-start`
- `.text-align-end`

### Text Decoration
Use the `.text-decoration-[variant]` class to apply text decoration.

**Template**: `<p class="text-decoration-underline">text</p>`

Available variants:
- `.text-decoration-underline`
- `.text-decoration-overline`
- `.text-decoration-line-through`
- `.text-decoration-none`

### Text Transformation
Use the `.text-transform-[variant]` class to transform text.

**Template**: `<p class="text-transform-uppercase">text</p>`

Available variants:
- `.text-transform-uppercase`
- `.text-transform-lowercase`
- `.text-transform-capitalize`
- `.text-transform-none`

### Text Size
Use the `.text-size-[variant]` class to set the font size.

**Template**: `<p class="text-size-md">text</p>`

Available variants:
- `.text-size-xs`
- `.text-size-sm`
- `.text-size-md`
- `.text-size-lg`

### Line Height
Use `.text-line-height-[variant]` to specify the line height.

**Template**: `<p class="text-size-md text-line-height-sm">text</p>`

Available variants:
- `.text-line-height-xs`
- `.text-line-height-sm`
- `.text-line-height-md`

---

## Margin and Padding Utility Classes

### Margin Auto
Use the `.ml-auto`, `.mr-auto`, or `.m-auto` classes for automatic margin adjustment.

### Directional Margin and Padding
Use the `.m-[value]`, `.p-[value]` classes for specific margin and padding adjustments.

**Example**:
```html
<div class="mr-30">text</div>
<div class="p-30">text</div>
```

---

## Layout Width Utility Classes
Use the `.min-w-[value]`, `.max-w-[value]`, and `.w-[value]` classes for width adjustments.

**Example**:
```html
<div class="min-w-xl">Minimum width of 800px</div>
```

---

## Display, Align Items, and Justify Content
Use `.display-[value]`, `.ai-[value]`, and `.jc-[value]` for display, alignment, and justification.

**Example**:
```html
<div class="display-flex jc-center ai-center">
  <p>Centered content in a flex container.</p>
</div>
```

---

## Cursor Utility Classes
Use the `.cursor-[value]` class to apply cursor styles.

**Example**:
```html
<div class="cursor-pointer">Clickable element</div>
```

---

## Border and Rounded Utility Classes
Use `.rounded-[value]`, `.border-color-[value]`, `.border-width-[value]`, and `.border-style-[value]` for border and rounded corner styles.

**Example**:
```html
<div class="rounded-sm border-width-1 border-color-grey-1 border-style-solid">
  Box with small rounded corners, 1px grey solid border.
</div>
```

---

## Background Color Utility Classes
Use the `.bg-color-[value]` class to set background colors.

**Example**:
```html
<div class="bg-color-grey-5">This div has a grey background.</div>
```

---

## Button Utility Classes
Use `.btn-min-height-[value]`, `.btn-min-width-[value]`, and `.btn-line-height-[value]` for button size and line height.

**Example**:
```html
<div class="btn btn-min-height-md btn-min-width-md">Button</div>
```

---

## Fill Utility Classes
Use the `.fill-[value]` class to apply fill colors, typically for SVGs.

**Example**:
```html
<svg class="fill-grey-5"></svg>
```

---

## CSS Functions

### `em()` function
Converts pixel values to `em` units based on the parent context.

```scss
@function em($pixels, $context: $browser-context) {
  @if (unitless($pixels)) {
    $pixels: $pixels * 1px;
  }
  @if (unitless($context)) {
    $context: $context * 1px;
  }
  @return calc($pixels / $context) * 1em;
}
```

### `rem()` function
Converts pixel values to `rem` units based on the root context.

```scss
@function rem($pixels) {
  $context: $browser-context;
  @if (unitless($pixels)) {
    $pixels: $pixels * 1px;
  }
  @if (unitless($context)) {
    $context: $context * 1px;
  }
  @return calc($pixels / $context)+rem;
}
```

---

