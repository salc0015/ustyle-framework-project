# UStyle CSS Framework

**UStyle** is a responsive and customizable CSS framework built using **Sass** and organized through **Sass partials**. It is designed to help developers and designers rapidly prototype and build visually consistent websites by offering utility classes, modular theming, and clean base styling for standard HTML elements.

---

## Authors

**UStyle** was created as part of an academic project focused on CSS architecture, modular design systems, and Sass-based development.

Created by:  
- Karen Melissa Flores Herrera  
- Viviana Gonzalez Moreno  
- Dalia Salcedo Nunez

---

## Overview

UStyle provides a **theme-first approach** to styling, with centralized variables and utility classes for layout, spacing, colors, and typography. It is fully built with Sass to allow **easy user customization** through maps and variables, while ensuring scalability and maintainability across projects.

---

## 📁 Project Structure

```
USTYLE-FRAMEWORK-PROJECT/
│
├── index.html            # HTML sample using the framework
├── css/
│   └── ustyle-style.css  # Compiled CSS output
└── src/
    ├── main.scss         # Main Sass entry point
    ├── base/             # Base styles and components
    │   ├── _align_.scss
    │   ├── _buttons.scss
    │   ├── _flex.scss
    │   ├── _forms.scss
    │   ├── _images.scss
    │   ├── _justiy.scss
    │   ├── _layout.scss
    │   ├── _links.scss
    │   ├── _lists.scss
    │   ├── _reset.scss
    │   ├── _rethink-sans.scss
    │   ├── _roboto.scss
    │   ├── _tables.scss
    │   ├── index.scss
    └── variables/        # Design tokens and theme settings
    │   ├── _colors_.scss
    │   ├── _theme.scss
    │   ├── _sizing.scss
    │   ├── _radius.scss
    │   ├── _background.scss
    │   └── _typography.scss
```



---

## Features

- **Built with Sass & Sass Partials**  
  All styles are organized using partials for better modularity and reuse.

- **Custom Theming**  
  Global color palette and theme roles (`primary`, `secondary`, `info`, etc.) defined in Sass maps.

- **Utility Classes**  
  For spacing, alignment, typography, layout (flexbox), color, and sizing.

- **Base Styling for Standard HTML Elements**  
  Forms, tables, headings, lists, links, and images have consistent styling applied using theme colors and spacing utilities.

- **User Customization**  
  Modify Sass variables or theme maps in `/src/variables/` to update colors, spacing, font sizes, etc.

- **Consistent & Cohesive Design**  
  When applied together, components and utility classes maintain a visually balanced interface.

- **Modern Sass Syntax**  
  Uses @use and @forward for modular and maintainable stylesheets.

---

## Installation

To install and start using the UStyle CSS Framework:

### 1. Clone or Download

```bash
git clone https://github.com/your-username/ustyle-framework.git
```

### 2. Link Compiled CSS

Include the compiled CSS file in your HTML file:

```html
<link rel="stylesheet" href="./css/ustyle-style.css">
```

### 3. Compile Sass (If You Customize)

If you change any Sass files inside /src, recompile them with:

```bash
sass --watch src/main.scss css/ustyle-style.css
```

---


## Usage

Use utility classes and component styles in your HTML just like with other CSS frameworks.

### Buttons

```html
<button class="btn-primary">Primary</button>
<a href="#" class="btn-pink">Link Button</a>
```

### Typography

```html
<h1 class="text-primary font-sz-3xl">Heading</h1>
<p class="text-dark font-sz-sm">Paragraph text</p>
```

### Spacing Utilities

```html
<div class="p-4 mb-3">Box with padding and margin</div>
```

### Layout with Flexbox

```html
<div class="flex flex-wrap gap-3 justify-center align-center">
  <div class="box-150 bg-primary"></div>
  <div class="box-150 bg-secondary"></div>
</div>
```

### Forms
```html
<form>
  <label for="name">Name</label>
  <input type="text" id="name" class="p-3">

  <label for="message">Message</label>
  <textarea id="message" class="p-3"></textarea>

  <button type="submit" class="btn-success">Send</button>
</form>
```
---

## Customization

You can easily customize the framework by editing Sass maps and variables in the `/src/variables/` folder:

- **_colors.scss** – Define all available colors  
- **_theme.scss** – Assign colors to roles like `primary`, `danger`, `info`, etc.  
- **_sizing.scss** – Manage spacing (`$spacing`), sizing (`$fixed-sizes`, `$width`), and responsive classes  
- **_typography.scss** – Set up font families, weights, and generate font-size classes  

After making your changes, recompile with:

```bash
sass src/main.scss css/ustyle-style.css
```

---
## Tips

- Utility classes like `.w-150`, `.h-100`, `.gap-3`, `.radius-md`, `.text-success` are generated dynamically from Sass maps.
-You can apply consistent styling by combining utilities like `.box-150`, `.font-sz-xl`, `.radius-lg`, and `.bg-primary`.
-Typography, layout spacing, background colors, and button styles are all mapped to variables and updated globally.
- The design system is scalable: just update your variables and everything updates across the framework.
- All default HTML elements are styled to look cohesive without needing additional CSS.

---
## Live Demo

Open `index.html` in your browser to see a sample page demonstrating all core features and utility classes in action.

---
## Requirements

- Sass installed (`npm install -g sass`) or use the **Live Sass Compiler** extension in your IDE.
- A modern browser for previewing changes.
- Basic understanding of Sass and HTML.
- Dart Sass is recommended to support @use and @forward syntax.

---
## License

This project is open source and free for personal and educational use.