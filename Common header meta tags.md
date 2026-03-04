# Technical Paper on Common Header Meta Tags in HTML

## 1. Introduction

Meta tags are placed inside the `<head>` section of an HTML document.

They provide information about the webpage.

Meta tags are not visible on the webpage, but they are important for:

- Browser settings  
- Search engines  
- Responsive design  
- Character encoding  

---

## 2. Basic Structure

Meta tags are written inside the `<head>` tag.

```html
<!DOCTYPE html>
<html>
<head>
  <meta>
</head>
<body>
</body>
</html>
```

---

## 3. Common Header Meta Tags

### 3.1 Character Set (charset)

Defines the character encoding of the webpage.

```html
<meta charset="UTF-8">
```

UTF-8 supports most languages and symbols.

---

### 3.2 Viewport (Responsive Design)

Used to make the website responsive on mobile devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

- `width=device-width` → matches screen width  
- `initial-scale=1.0` → normal zoom level  

---

### 3.3 Description

Provides a short description of the webpage.  
Used by search engines.

```html
<meta name="description" content="This is a website about learning HTML and CSS.">
```

---

### 3.4 Keywords

Defines keywords related to the webpage.

```html
<meta name="keywords" content="HTML, CSS, Web Design">
```

---

### 3.5 Author

Defines the author of the webpage.

```html
<meta name="author" content="Abhay Sharma">
```

---

### 3.6 Refresh

Automatically refreshes the page after a given time.

```html
<meta http-equiv="refresh" content="5">
```

This refreshes the page after 5 seconds.

---

## 4. Complete Example

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Learning HTML meta tags">
  <meta name="keywords" content="HTML, CSS, Meta Tags">
  <meta name="author" content="Abhay Sharma">
  <title>Meta Tag Example</title>
</head>
<body>

<h1>Meta Tags Example</h1>

</body>
</html>
```

---

## 5. Conclusion

Meta tags are important for webpage settings and SEO.

Common meta tags are:

- charset  
- viewport  
- description  
- keywords  
- author  
- refresh  

They help browsers and search engines understand the webpage.