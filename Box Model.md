# Technical Paper on CSS Box Model

## 1. Introduction

In CSS, every HTML element is treated like a rectangular box.  
This structure is called the **Box Model**.

The box model helps us understand spacing and size of elements on a web page.

The CSS Box Model has four parts:

- Content  
- Padding  
- Border  
- Margin  

---

## 2. Parts of the Box Model

### 2.1 Content

Content is the actual text, image, or data inside the element.

Example:

```css
div {
  width: 200px;
  height: 100px;
}
```

---

### 2.2 Padding

Padding is the space between content and border.  
It increases the total size of the element.

```css
div {
  padding: 20px;
}
```

---

### 2.3 Border

Border goes around the padding and content.

```css
div {
  border: 3px solid black;
}
```

---

### 2.4 Margin

Margin is the space outside the border.  
It creates space between elements.

```css
div {
  margin: 30px;
}
```

---

## 3. Total Width and Height Calculation

By default, CSS uses `content-box`.

Total width is calculated as:

```
Total Width = width + left padding + right padding + left border + right border
```

Example:

```css
div {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
}
```

Total width becomes:

```
200 + 20 + 20 + 5 + 5 = 250px
```

---

## 4. box-sizing Property

### content-box (Default)

Width and height apply only to content.

```css
div {
  box-sizing: content-box;
}
```

### border-box

Width includes content, padding, and border.

```css
div {
  box-sizing: border-box;
}
```

This is commonly used in modern websites because it keeps the total width fixed.

---

## 5. Complete Example (HTML + CSS)

```html
<!DOCTYPE html>
<html>
<head>
<style>
.box {
  width: 200px;
  padding: 20px;
  border: 5px solid blue;
  margin: 30px;
  background-color: lightgray;
  box-sizing: border-box;
}
</style>
</head>
<body>

<div class="box">
  This is a Box Model example
</div>

</body>
</html>
```

---

## 6. Conclusion

The CSS Box Model is very important in web design.  
It helps control spacing and layout of elements.

Every element follows this order:

Content → Padding → Border → Margin