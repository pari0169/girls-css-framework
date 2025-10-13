# girls-css-framework
Our team will create a efficient framework for modern website.

A custom CSS framework built by our team for the “Custom CSS Framework” project.  
This framework is built with **Sass partials** and provides a **consistent custom theme** for standard HTML elements such as headings, lists, buttons, forms, inputs, and tables.  
It also includes **utility classes** for quick and flexible styling across color, font weight, font size, margin, padding, and borders.

---

## Features

- **Built with Sass and Sass partials** for organized, modular code.  
- **Customizable variables** for easy theme changes (colors, spacing, fonts).  
- **Themed elements** including:
  - Headings and typography
  - Lists (unstyled, inline, and check list)
  - Buttons (primary, secondary, accent, ghost)
  - Forms and inputs (with states and help text)
  - Tables (striped, bordered)
- **Utility classes** for:
  - Spacing (`u-m-1`, `u-p-2`, etc.)
  - Font weight and size (`u-fw-700`, `u-fs-lg`, etc.)
  - Colors (`u-text-primary`, `u-bg-accent`, etc.)
  - Borders (`u-border`, `u-rounded-md`, etc.)
- **Compiled CSS** file ready to use in `dist/`.

---

###Installation & Build

### Requirements
Make sure you have **Node.js** and **Sass** installed.

### Steps
```bash
# Clone the repository
git clone https://github.com/pari0169/girls-css-framework.git
cd girls-css-framework

# Install Sass if you don't have it
npm install --save-dev sass

# Build once
npx sass scss/style.scss dist/style.css --style=expanded

# Or build and watch for changes
npx sass --watch scss/style.scss dist/style.css --style=expanded

### Usage

To use the framework in your website, link the compiled CSS file inside your HTML:

<link rel="stylesheet" href="dist/style.css">

### Customization

You can change the theme by overriding Sass variables before compiling.

Then import it before the main file:

@use "overrides";
@use "style";

Rebuild the CSS file to apply your new styles:

npx sass scss/style.scss dist/style.css --style=expanded