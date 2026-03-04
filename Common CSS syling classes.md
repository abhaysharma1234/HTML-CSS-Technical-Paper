# Technical Paper on Common CSS Styling Classes

## 1. Introduction

CSS styling classes are used to change the appearance of elements.

They control:

- Colors  
- Text style  
- Size  
- Spacing  
- Background  
- Borders  

These classes help make the website look attractive.

---

## 2. Common CSS Styling Classes

Below are some commonly used styling classes.

---

### 2.1 Text Color Classes

Used to change text color.

```css
.text-red {
  color: red;
}

.text-blue {
  color: blue;
}
```

Usage:

```html
<p class="text-red">This is red text</p>
```

---

### 2.2 Background Color Classes

Used to change background color.

```css
.bg-yellow {
  background-color: yellow;
}

.bg-light {
  background-color: lightgray;
}
```

Usage:

```html
<div class="bg-light">Background Example</div>
```

---

### 2.3 Text Alignment Classes

Used to align text.

```css
.text-center {
  text-align: center;
}

.text-right {
  text-align: right;
}
```

Usage:

```html
<p class="text-center">Centered Text</p>
```

---

### 2.4 Font Size Classes

Used to change text size.

```css
.small {
  font-size: 12px;
}

.large {
  font-size: 24px;
}
```

Usage:

```html
<p class="large">Large Text</p>
```

---

### 2.5 Margin and Padding Classes

Used to control spacing.

```css
.m-20 {
  margin: 20px;
}

.p-10 {
  padding: 10px;
}
```

Usage:

```html
<div class="m-20 p-10">Spacing Example</div>
```

---

### 2.6 Border Classes

Used to add borders.

```css
.border {
  border: 2px solid black;
}

.round {
  border-radius: 10px;
}
```

Usage:

```html
<div class="border round">Border Example</div>
```

---

## 3. Complete Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
.text-red { color: red; }
.bg-light { background-color: lightgray; }
.text-center { text-align: center; }
.large { font-size: 24px; }
.m-20 { margin: 20px; }
.p-10 { padding: 10px; }
.border { border: 2px solid black; }
.round { border-radius: 10px; }
</style>
</head>
<body>

<div class="bg-light m-20 p-10 border round">
  <p class="text-red large text-center">
    Common CSS Styling Classes Example
  </p>
</div>

</body>
</html>
```

---

## 4. Conclusion

Common CSS styling classes help improve the design of a website.

They are used to control:

- Text color  
- Background  
- Alignment  
- Font size  
- Spacing  
- Borders  

