# Technical Paper on CSS Specificity

## 1. Introduction

CSS Specificity decides which CSS rule will apply when multiple rules target the same element.

When two or more styles are applied to the same element, the browser uses specificity to choose the stronger rule.

---

## 2. Types of Selectors and Their Priority

CSS selectors have different priority levels.

### 2.1 Inline Style (Highest Priority)

Inline style has the highest specificity.

Example:

```html
<p style="color: red;">This is a paragraph</p>
```

This will override most other styles.

---

### 2.2 ID Selector

ID selectors have high priority.

```css
#para {
  color: blue;
}
```

Usage:

```html
<p id="para">Hello</p>
```

---

### 2.3 Class Selector

Class selectors have medium priority.

```css
.text {
  color: green;
}
```

Usage:

```html
<p class="text">Hello</p>
```

---

### 2.4 Element Selector (Lowest Priority)

Element selectors have the lowest priority.

```css
p {
  color: black;
}
```

---

## 3. Specificity Order (High to Low)

1. Inline Style  
2. ID Selector  
3. Class Selector  
4. Element Selector  

---

## 4. Example of Specificity

```html
<!DOCTYPE html>
<html>
<head>
<style>
p {
  color: black;
}

.text {
  color: green;
}

#para {
  color: blue;
}
</style>
</head>
<body>

<p id="para" class="text">
  This text will be blue.
</p>

</body>
</html>
```

Explanation:

- Element selector sets color to black.
- Class selector sets color to green.
- ID selector sets color to blue.
- ID has higher priority, so text becomes blue.

---

## 5. Important Rule (!important)

The `!important` rule overrides all other styles.

```css
p {
  color: red !important;
}
```

This will apply even if other selectors have higher priority.

Use `!important` carefully.

---

## 6. Conclusion

CSS Specificity decides which style is applied.

Priority order:

Inline > ID > Class > Element
