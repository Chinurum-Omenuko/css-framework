# LADLE CSS FRAMEWORK

## Team Members

[Your team details here]

---

## INSTALLATION

```bash
npm install ladle-css
```

Or include the compiled CSS in your HTML:

```html
<link rel="stylesheet" href="path-to/ladle.css" />
```

---

## FEATURES

- **Responsive Grid System**: 12-column grid with flexible gutter spacing.
- **Typography Utilities**: Predefined heading sizes, font weights, and text colors.
- **Forms**: Stylized inputs, checkboxes, radio buttons, and select boxes.
- **Buttons**: Predefined button styles, including disabled states.
- **Flexbox Layout**: Predefined flex classes for layout customization.
- **Utility Classes**: Padding, margin, background, border, and text utilities.
- **Animations**: Simple predefined animations like opacity, reveal, and slide effects.

---

## USAGE

### Typography

Ladle CSS provides an easy way to handle typography. Use heading tags (`<h1>` to `<h6>`) to apply preset styles for titles.

```html
<h1 class="text-primary text-center mb-3">Ladle CSS Framework</h1>
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h6>
<p>This is a paragraph of text. <span class="text-secondary">This is inline text.</span></p>
```

---

### Links & Buttons

Easily create links and buttons with Ladle's predefined classes.

```html
<a href="#" class="text-primary">Primary Link</a><br />
<button class="btn">Default Button</button>
<button class="btn btn-primary">Primary Button</button>
<button class="btn btn-secondary">Secondary Button</button>
<button class="btn btn-disabled" disabled>Disabled Button</button>
```

---

### Forms

Ladle CSS makes it easy to style form elements. The following example demonstrates a basic form setup with input fields, checkboxes, radio buttons, and select boxes.

```html
<form class="flex flex-column gap-1">
  <div class="form-group">
    <label for="input-text">Text Input:</label>
    <input type="text" id="input-text" class="input" />
  </div>

  <div class="form-group">
    <label for="checkbox">Checkbox:</label>
    <input type="checkbox" id="checkbox" class="checkbox" />
  </div>

  <div class="form-group">
    <label for="radio">Radio Button:</label>
    <input type="radio" id="radio" name="radio" class="radio" />
  </div>

  <div class="form-group">
    <label for="select">Select Box:</label>
    <select id="select" class="select">
      <option>Option 1</option>
      <option>Option 2</option>
    </select>
  </div>

  <div class="form-actions">
    <button type="submit" class="btn btn-primary">Submit</button>
    <button type="reset" class="btn btn-secondary">Reset</button>
  </div>
</form>
```

---

### Grid Layout

Ladle CSS provides a powerful and flexible grid system. You can create responsive layouts using `col-x-12` classes, where x represents the number of columns.

```html
<div class="grid">
  <div class="col-4-12 bg-primary text-white">4/12 Column</div>
  <div class="col-4-12 bg-secondary text-white">4/12 Column</div>
  <div class="col-4-12 bg-green text-white">4/12 Column</div>
</div>
<div class="grid">
  <div class="col-6-12 bg-primary text-white">6/12 Column</div>
  <div class="col-6-12 bg-secondary text-white">6/12 Column</div>
</div>
```

---

### Flexbox Layout

The framework comes with built-in flexbox utilities for responsive and flexible layouts.

```html
<div class="flex flex-row justify-between items-center text-white">
  <div class="box bg-primary">Flex Item 1</div>
  <div class="box bg-secondary">Flex Item 2</div>
  <div class="box bg-green">Flex Item 3</div>
</div>
```

---

### Utilities

Ladle CSS has several utility classes that help with spacing, text, background, and borders.

```html
<div class="bg-primary text-white p-4">Padding Utility</div>
<div class="bg-secondary text-white m-4 p-4">Margin Utility</div>
<div class="bg-tertiary text-white border p-4">Border Utility</div>
<div class="bg-primary text-white text-decoration-underline p-4">
  Underline Text
</div>
```

---

### Animations

Ladle CSS supports a few simple animations for basic effects like opacity, slide, and reveal.

```html
<div class="flex flex-row gap-2">
  <div class="box bg-primary text-white p-10 animate-opacity loop">Opacity</div>
  <div class="box bg-secondary text-white p-10 animate-reveal loop">Reveal</div>
  <div class="box bg-green text-white p-10 animate-slide loop">Slide</div>
</div>
```

---

## CUSTOMIZATION OPTIONS

Ladle CSS is built with modularity in mind. To customize the framework, simply modify the variables in the `ladle.scss` file to adjust colors, spacing, and font settings.

Example:

```scss
$primary-color: #3498db;
$secondary-color: #f1c40f;
$font-family: "Montserrat", sans-serif;
```

---

## DEVELOPMENT

Ladle CSS is built using Sass. To watch for changes and automatically recompile the CSS, use the following command:

```bash
sass --watch src/main.scss css/ladle.css
```

For developers looking to expand on the existing framework, feel free to extend the `main.scss` file and modify components as needed for your projects.
