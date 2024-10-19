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
