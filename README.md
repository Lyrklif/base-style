# CSS Text Utility Classes
Basic SCSS styles for any frontend project


## Text Color
Use the `.text-color-[variant]` class to apply different text colors.

**Template**: `<p class="text-color-blue">text</p>`

Available variants:
- `.text-color-[variant]`: Apply the specific color to text.

## Text Font Family
Use the `.text-ff-[variant]` class to set the font family.

**Template**: `<p class="text-ff-secondary">text</p>`

Available variants:
- `.text-ff-primary`: Uses the primary font family.
- `.text-ff-secondary`: Uses the secondary font family.

## Text Weight
Use the `.text-weight-[variant]` class to set the font weight.

**Template**: `<p class="text-weight-bold">text</p>`

Available variants:
- `.text-weight-regular`
- `.text-weight-medium`
- `.text-weight-semibold`
- `.text-weight-bold`

## Text Alignment
Use the `.text-align-[variant]` class to align text.

**Template**: `<p class="text-align-center">text</p>`

Available variants:
- `.text-align-left`
- `.text-align-center`
- `.text-align-right`
- `.text-align-justify`
- `.text-align-start`
- `.text-align-end`

## Text Decoration
Use the `.text-decoration-[variant]` class to apply text decoration.

**Template**: `<p class="text-decoration-underline">text</p>`

Available variants:
- `.text-decoration-underline`
- `.text-decoration-overline`
- `.text-decoration-line-through`
- `.text-decoration-none`

## Text Transformation
Use the `.text-transform-[variant]` class to transform text.

**Template**: `<p class="text-transform-uppercase">text</p>`

Available variants:
- `.text-transform-uppercase`
- `.text-transform-lowercase`
- `.text-transform-capitalize`
- `.text-transform-none`

## Text Size
Use the `.text-size-[variant]` class to set the font size.

**Template**: `<p class="text-size-md">text</p>`

Available variants:
- `.text-size-xs`
- `.text-size-sm`
- `.text-size-md`
- `.text-size-lg`

### Line Height for Text Sizes
Within `.text-size-[variant]` classes, use `.text-line-height-[variant]` to specify the line height for the text size.

**Template**: `<p class="text-size-md text-line-height-sm">text</p>`

Available variants:
- `.text-line-height-xs`
- `.text-line-height-sm`
- `.text-line-height-md`

## Line Height (Simple)
Use the `.text-line-height-[variant]` class to set a simple line height.

**Template**: `<p class="text-line-height-normal">text</p>`

Available variants:
- `.text-line-height-normal`
- `.text-line-height-inherit`
- `.text-line-height-initial`
- `.text-line-height-none`

---

## Offset Variants
The following offset variants are defined to represent margin and padding:

```scss
$offset-name-variants: (
  'm': 'margin',
  'p': 'padding',
);
```

## Margin Variants
The following margin variants are available:

```scss
$margin-variants: (
 '0': 0px,
 '30': 30px,
);
```

## Utility Classes

### Margin Auto
- `.ml-auto`: Sets `margin-left` to `auto`.
- `.mr-auto`: Sets `margin-right` to `auto`.
- `.m-auto`: Sets both `margin-left` and `margin-right` to `auto`.

### Margin Classes
Use the `.m-[value]`, `.my-[value]`, `.mx-[value]`, `.mt-[value]`, `.mb-[value]`, `.ml-[value]`, and `.mr-[value]` classes to apply margin:

**Templates**:
- `<div class="mr-30">text</div>`: Sets `margin-right` to `30px`.
- `<div class="my-0">text</div>`: Sets vertical margins (top and bottom) to `0px`.
- `<div class="pr-30">text</div>`: Sets `padding-right` to `30px`.
- `<div class="p-30">text</div>`: Sets all padding to `30px`.

### Margin/Padding Directional Classes
- **Y-axis (Vertical)**:
    - `.my-[value]`: Sets top and bottom margin.
- **X-axis (Horizontal)**:
    - `.mx-[value]`: Sets left and right margin.
- **Top**:
    - `.mt-[value]`: Sets `margin-top`.
- **Bottom**:
    - `.mb-[value]`: Sets `margin-bottom`.
- **Left**:
    - `.ml-[value]`: Sets `margin-left`.
- **Right**:
    - `.mr-[value]`: Sets `margin-right`.

## Example Usage
```html
<div class="mr-30">text</div>
<div class="my-0">text</div>
<div class="pr-30">text</div>
<div class="p-30">text</div>
```


## Width Property Variants
The following width property variants are defined:

```scss
$layout-width-property-variants: (
  'min-w': 'min-width',
  'max-w': 'max-width',
  'w': 'width',
);
```

## Width Variants
The following width variants are available:

```scss
$layout-width-variants: (
  'xl': 800px,
  'xxl': 1200px,
);
```

## Utility Classes
The following utility classes can be used to apply widths:

### Width Classes
Use the `.min-w-[value]`, `.max-w-[value]`, and `.w-[value]` classes to apply specific widths:

**Templates**:
- `<div class="min-w-xl">text</div>`: Sets the `min-width` to `800px`.
- `<div class="max-w-xxl">text</div>`: Sets the `max-width` to `1200px`.
- `<div class="w-xl">text</div>`: Sets the `width` to `800px`.

## Example Usage
```html
<div class="min-w-xl">Minimum width of 800px</div>
<div class="max-w-xxl">Maximum width of 1200px</div>
<div class="w-xl">Width of 800px</div>
```

---


## Display Variants
The following display variants are defined:

```scss
$display-variants: [ 'block', 'inline-block', 'inline', 'flex', 'inline-flex', 'none' ];
```

## Align Items Variants
The following align-items variants are available:

```scss
$align-items-variants: (
  'start': 'flex-start',
  'end': 'flex-end',
  'center': 'center',
  'baseline': 'baseline',
  'stretch': 'stretch',
);
```

## Justify Content Variants
The following justify-content variants are available:

```scss
$justify-content-variants: (
  'start': 'flex-start',
  'end': 'flex-end',
  'center': 'center',
  'between': 'space-between',
  'around': 'space-around',
  'evenly': 'space-evenly',
);
```

## Utility Classes

### Display Classes
Use the `.display-[value]` classes to apply specific display types:

**Templates**:
- `<div class="display-block"></div>`: Sets the display to `block`.
- `<div class="display-inline"></div>`: Sets the display to `inline`.
- `<div class="display-flex"></div>`: Sets the display to `flex`.

### Align Items Classes
Use the `.ai-[value]` classes to align items in flex containers:

**Templates**:
- `<p class="ai-start">text</p>`: Aligns items to the start.
- `<p class="ai-center">text</p>`: Centers the items vertically.

### Justify Content Classes
Use the `.jc-[value]` classes to justify content in flex containers:

**Templates**:
- `<p class="jc-start">text</p>`: Justifies content to the start.
- `<p class="jc-center">text</p>`: Centers the content horizontally.
- `<p class="jc-between">text</p>`: Distributes space between items evenly.

## Example Usage
```html
<div class="display-flex jc-center ai-center">
  <p>Centered content in a flex container.</p>
</div>
```

---


## Cursor Variants
The following cursor variants are defined:

```scss
$cursor-variants: [ 'auto', 'default', 'pointer', 'wait', 'text', 'not-allowed', 'none' ];
```

## Utility Classes

Use the `.cursor-[value]` classes to apply specific cursor styles:

### Cursor Classes
- `.cursor-auto`: Sets the cursor to `auto`.
- `.cursor-default`: Sets the cursor to `default`.
- `.cursor-pointer`: Sets the cursor to `pointer`, typically used for links and interactive elements.
- `.cursor-wait`: Sets the cursor to `wait`, indicating that the page or element is loading.
- `.cursor-text`: Sets the cursor to `text`, typically used for text inputs or editable text fields.
- `.cursor-not-allowed`: Sets the cursor to `not-allowed`, indicating that an action is not allowed.
- `.cursor-none`: Hides the cursor.

## Example Usage
```html
<div class="cursor-pointer">Clickable element</div>
<div class="cursor-text">Text input area</div>
<div class="cursor-not-allowed">Disabled element</div>
```

---

## Rounded Variants
The following rounded corner variants are defined:

```scss
$rounded-variants: (
  'none': $border-radius-none,
  'sm': $border-radius-sm,
  'md': $border-radius-md,
  'lg': $border-radius-lg,
  'full': $border-radius-full,
);
```

### Rounded Classes
Use the `.rounded-[value]` classes to apply specific border-radius values:

**Templates**:
- `<div class="rounded-sm"></div>`: Sets a small border-radius.
- `<div class="rounded-full"></div>`: Sets a full (circular) border-radius.

## Border Color Variants
The following border color variants are defined:

```scss
$border-color-variants: $full-color-variants;
```

### Border Color Classes
Use the `.border-color-[value]` classes to apply specific border colors:

**Templates**:
- `<div class="border-color-grey-1"></div>`: Sets the border color to grey.

## Border Width Variants
The following border width variants are defined:

```scss
$border-width-variants: (
  '0': 0px,
  '1': 1px,
  '2': 2px,
  '3': 3px,
);
```

### Border Width Classes
Use the `.border-width-[value]` classes to apply specific border widths:

**Templates**:
- `<div class="border-width-1"></div>`: Sets the border width to 1px.

## Border Style Variants
The following border style variants are defined:

```scss
$border-style-variants: [ 'solid', 'dashed', 'dotted', 'double', 'hidden', 'none' ];
```

### Border Style Classes
Use the `.border-style-[value]` classes to apply specific border styles:

**Templates**:
- `<div class="border-style-solid"></div>`: Sets the border style to solid.
- `<div class="border-style-dashed"></div>`: Sets the border style to dashed.

## Example Usage
```html
<div class="rounded-sm border-width-1 border-color-grey-1 border-style-solid">
  Box with small rounded corners, 1px grey solid border.
</div>
<div class="rounded-full border-width-2 border-color-blue border-style-dotted">
  Circular box with 2px blue dotted border.
</div>
```

---

## Background Color Variants
The following background color variants are defined:

```scss
$bg-color-variants: $full-color-variants;
```

### Background Color Classes
Use the `.bg-color-[value]` classes to apply specific background colors:

**Templates**:
- `<div class="bg-color-grey-5"></div>`: Sets the background color to a specific shade of grey.

## Example Usage
```html
<div class="bg-color-grey-5">
  This div has a grey background.
</div>
<div class="bg-color-blue">
  This div has a blue background.
</div>
```

---


## Button Min Height Variants
The following minimum height variants are defined:

```scss
$btn-min-height-variants: (
  'md': 55px,
  'lg': 60px,
);
```

### Button Min Height Classes
Use the `.btn-min-height-[value]` classes to apply specific minimum heights to buttons:

**Templates**:
- `<div class="btn-min-height-md"></div>`: Sets the minimum height to 55px.
- `<div class="btn-min-height-lg"></div>`: Sets the minimum height to 60px.

## Button Min Width Variants
The following minimum width variants are defined:

```scss
$btn-min-width-variants: (
  'sm': 60px,
  'md': 200px,
);
```

### Button Min Width Classes
Use the `.btn-min-width-[value]` classes to apply specific minimum widths to buttons:

**Templates**:
- `<div class="btn-min-width-sm"></div>`: Sets the minimum width to 60px.
- `<div class="btn-min-width-md"></div>`: Sets the minimum width to 200px.

## Button Line Height Variants
The line-height classes follow the same values as min-height variants.

### Button Line Height Classes
Use the `.btn-line-height-[value]` classes to apply specific line heights to buttons:

**Templates**:
- `<div class="btn-line-height-md"></div>`: Sets the line-height to 55px.
- `<div class="btn-line-height-lg"></div>`: Sets the line-height to 60px.

## Example Usage
```html
<div class="btn btn-min-height-md btn-min-width-md">
  Button with minimum height 55px and minimum width 200px.
</div>
<div class="btn btn-min-height-lg btn-line-height-lg">
  Button with larger height and matching line height.
</div>
```

---


## Fill Color Variants
The following fill color variants are defined:

```scss
$full-color-variants: $full-color-variants;
```

### Fill Classes
Use the `.fill-[value]` classes to apply specific fill colors:

**Templates**:
- `<p class="fill-black">text</p>`: Sets the fill color to black.

## Example Usage
```html
<p class="fill-black">Black fill applied</p>
<p class="fill-blue">Blue fill applied</p>
<svg class="fill-grey-5">
  <!-- SVG content -->
</svg>
```

---


The `em()` function is a utility that converts pixel values to `em` units, which are relative to the font size of the parent element (or the context). It can be used for setting font sizes and other CSS properties in a scalable and responsive manner.

## Function Definition

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

### Parameters:
- **$pixels**: The pixel value you want to convert to `em`. It can be unitless or in pixels.
- **$context** (optional): The context in which the `em` value is calculated. By default, it's set to the browser's base font size (usually `16px`).

### Return:
- The function returns the equivalent value in `em` units as calculated relative to the context.

## Usage

You can use the `em()` function to convert pixel-based values into `em` units in your styles.

### Example:

**Template**:
```scss
font-size: em(18);
// Equivalent to:
font-size: em(18px);
```

**Result**:
- Converts `18px` to `em` based on the context (default `16px`), resulting in a font size of `1.125em`.

---


The `rem()` function is a utility that converts pixel values to `rem` units, which are relative to the root element’s font size (usually `16px` by default). It can be used for setting font sizes and other CSS properties in a scalable and responsive manner.

## Function Definition

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

### Parameters:
- **$pixels**: The pixel value you want to convert to `rem`. It can be unitless or in pixels.

### Return:
- The function returns the equivalent value in `rem` units as calculated relative to the browser's root font size (default is `16px`).

## Usage

You can use the `rem()` function to convert pixel-based values into `rem` units in your styles.

### Example:

**Template**:
```scss
font-size: rem(18);
// Equivalent to:
font-size: rem(18px);
```

**Result**:
- Converts `18px` to `rem` based on the root context (default `16px`), resulting in a font size of `1.125rem`.

---
