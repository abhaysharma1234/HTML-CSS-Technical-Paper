# Technical Paper on Common CSS Structural Classes

## 1. Introduction

CSS structural classes are commonly used class names that help in designing the layout of a web page.

These classes are used to organize content properly and make the design clean.

They are not fixed by CSS. Developers create them based on need.

---

## 2. Common Structural Classes

Below are some commonly used structural classes.

---

### 2.1 container

The `container` class is used to wrap the whole content of the page.

It keeps content centered and gives fixed width.

```css
.container {
  width: 80%;
  margin: 0 auto;
}
```

---

### 2.2 header

The `header` class is used for the top section of the website.

```css
.header {
  background-color: lightblue;
  padding: 20px;
  text-align: center;
}
```

---

### 2.3 navbar

The `navbar` class is used for navigation links.

```css
.navbar {
  background-color: black;
  padding: 10px;
}

.navbar a {
  color: white;
  margin-right: 15px;
  text-decoration: none;
}
```

---

### 2.4 content

The `content` class is used for the main section of the page.

```css
.content {
  padding: 20px;
}
```

---

### 2.5 sidebar

The `sidebar` class is used for side content like links or ads.

```css
.sidebar {
  width: 25%;
  float: right;
  background-color: lightgray;
  padding: 15px;
}
```

---

### 2.6 footer

The `footer` class is used for the bottom section of the website.

```css
.footer {
  background-color: black;
  color: white;
  text-align: center;
  padding: 15px;
}
```

---

## 3. Complete Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
.container {
  width: 80%;
  margin: 0 auto;
}

.header {
  background: lightblue;
  padding: 20px;
  text-align: center;
}

.navbar {
  background: black;
  padding: 10px;
}

.navbar a {
  color: white;
  margin-right: 15px;
  text-decoration: none;
}

.content {
  padding: 20px;
}

.footer {
  background: black;
  color: white;
  text-align: center;
  padding: 15px;
}
</style>
</head>
<body>

<div class="container">
  <div class="header">Header Section</div>
  
  <div class="navbar">
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </div>
  
  <div class="content">
    This is main content area.
  </div>
  
  <div class="footer">
    Footer Section
  </div>
</div>

</body>
</html>
```

---

## 4. Conclusion

Common CSS structural classes help organize the layout of a webpage.

Some common classes are:

- container  
- header  
- navbar  
- content  
- sidebar  
- footer  

They make the website structured and easy to design.