# Gridlight

**A lightweight, responsive 12-column CSS Grid framework built for simplicity.**  
No Flexbox. No JavaScript. Just clean CSS Grid, responsive classes, and full control.

---

## Why Gridlight?

Sometimes you just want to build layouts — without loading a 300KB framework or writing complex utility chains. Gridlight is made for that.

- Built with native CSS Grid  
- Mobile-first and responsive by default  
- Simple class system like `col-6`, `col-t-8`, `col-d-4`  
- No Flexbox, no JS, no dependencies  
- Customize everything using CSS variables

Perfect for designers, developers, and anyone who hates bloated boilerplate.

[Demo](https://biju001.github.io/Gridlight/)

---

## Getting Started

### 1. Add the CSS

```
<link rel="stylesheet" href="dist/gridlight.css" />
```

### 2. Create a layout

```
<div class="row">
  <div class="col-12 col-t-6 col-d-4">Block 1</div>
  <div class="col-12 col-t-6 col-d-4">Block 2</div>
  <div class="col-12 col-t-12 col-d-4">Block 3</div>
</div>
```
### Class Naming System

| Class      | Applies To         | Example     |
|------------|--------------------|-------------|
| `col-`     | Mobile <600px      | `col-6`     |
| `col-t-`   | Tablet ≥600px      | `col-t-8`   |
| `col-d-`   | Desktop ≥992px     | `col-d-4`   |


If a class isn’t defined for mobile or tablet, it falls back to the next available breakpoint.

## Customization

Gridlight uses CSS variables for spacing, fonts, colors, and breakpoints.

```
:root {
  --grid-gap: 3px;
  --font-family: 'Inter', sans-serif;
  --color-accent: #007BFF;
}
```

No-gap layout:
```
<div class="no-gap">
  <div class="row">
    <div class="col-6">No Gap</div>
    <div class="col-6">No Gap</div>
  </div>
</div>
```



## License

This project is open-source and available under the [MIT License](LICENSE).
