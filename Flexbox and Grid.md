# Technical Paper on CSS Flexbox and Grid

## 1. Introduction

Flexbox and Grid are modern CSS layout systems.

They help in arranging elements properly on a web page.

- Flexbox is used for one-dimensional layout (row or column).
- Grid is used for two-dimensional layout (rows and columns).

---

# 2. CSS Flexbox

Flexbox is used to arrange items in a row or column.

To use flexbox, we apply `display: flex;` on the parent.

## 2.1 Basic Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
.container {
  display: flex;
  background-color: lightgray;
}

.box {
  background-color: orange;
  padding: 20px;
  margin: 10px;
}
</style>
</head>
<body>

<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>

</body>
</html>
```

All boxes appear in one row.

---

## 2.2 Important Flexbox Properties

- `flex-direction` → row or column  
- `justify-content` → horizontal alignment  
- `align-items` → vertical alignment  

Example:

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

---

# 3. CSS Grid

Grid is used for two-dimensional layout.

To use grid, apply `display: grid;` on the parent.

## 3.1 Basic Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 10px;
}

.box {
  background-color: lightblue;
  padding: 20px;
}
</style>
</head>
<body>

<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>

</body>
</html>
```

This creates 3 equal columns.

---

## 3.2 Important Grid Properties

- `grid-template-columns` → number of columns  
- `grid-template-rows` → number of rows  
- `gap` → space between items  

---

# 4. Difference Between Flexbox and Grid

| Flexbox | Grid |
|----------|------|
| One-dimensional | Two-dimensional |
| Row OR column | Row AND column |
| Good for small layouts | Good for full page layout |

---

# 5. Conclusion

Flexbox and Grid are powerful layout tools in CSS.

Flexbox is best for simple row or column layouts.  
Grid is best for complex layouts with rows and columns.
