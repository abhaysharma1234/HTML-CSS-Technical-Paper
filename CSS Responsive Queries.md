# Technical Paper on CSS Responsive Queries (Media Queries)

## 1. Introduction

Responsive design means a website adjusts properly on different screen sizes like:

- Mobile  
- Tablet  
- Laptop  
- Desktop  

CSS Media Queries are used to make websites responsive.

---

## 2. What is a Media Query?

A media query applies CSS only when a certain condition is true.

It is mostly used with screen width.

Basic syntax:

```css
@media (condition) {
  /* CSS code */
}
```

---

## 3. Example Using max-width

This example changes background color when screen width is 600px or less.

```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

Meaning:
- If screen width is 600px or smaller,
- Background becomes light blue.

---

## 4. Example Using min-width

```css
@media (min-width: 768px) {
  body {
    background-color: lightgreen;
  }
}
```

Meaning:
- If screen width is 768px or more,
- Background becomes light green.

---

## 5. Complete Responsive Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
.box {
  width: 400px;
  height: 200px;
  background-color: orange;
  text-align: center;
  line-height: 200px;
  margin: 20px auto;
}

/* For small screens */
@media (max-width: 600px) {
  .box {
    width: 200px;
    background-color: lightblue;
  }
}
</style>
</head>
<body>

<div class="box">
  Responsive Box
</div>

</body>
</html>
```

Explanation:

- On large screens → width is 400px.
- On small screens (600px or less) → width becomes 200px.

---

## 6. Common Breakpoints

Developers often use these screen sizes:

- 600px → Mobile  
- 768px → Tablet  
- 1024px → Small laptop  
- 1200px → Desktop  

---

## 7. Conclusion

CSS Media Queries help create responsive websites.

They allow CSS to change based on screen size.

This makes websites look good on all devices.