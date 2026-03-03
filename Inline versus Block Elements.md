# Technical Paper on Inline vs Block Elements in HTML

## 1. Introduction

In HTML, elements are divided into two main types:

- Block Elements  
- Inline Elements  

Understanding these elements is important for designing web pages correctly.

---

## 2. Block Elements

Block elements take the full width available.  
They always start on a new line.

### Features of Block Elements

- Start on a new line  
- Take full width  
- Can contain inline and block elements  
- Width and height can be set  

### Examples of Block Elements

- `<div>`
- `<p>`
- `<h1>` to `<h6>`
- `<section>`
- `<article>`

### Example Code

```html
<!DOCTYPE html>
<html>
<body>

<div>This is a div element</div>
<p>This is a paragraph</p>
<h1>This is a heading</h1>

</body>
</html>
```

Each element appears on a new line.

---

## 3. Inline Elements

Inline elements do not start on a new line.  
They take only the width required for their content.

### Features of Inline Elements

- Do not start on a new line  
- Take only required width  
- Cannot contain block elements  
- Width and height cannot be set properly  

### Examples of Inline Elements

- `<span>`
- `<a>`
- `<strong>`
- `<em>`
- `<img>`

### Example Code

```html
<!DOCTYPE html>
<html>
<body>

<span>This is span</span>
<a href="#">This is link</a>
<strong>This is bold text</strong>

</body>
</html>
```

All elements appear on the same line.

---

## 4. Comparison Table

| Block Element | Inline Element |
|---------------|----------------|
| Starts on new line | Does not start on new line |
| Takes full width | Takes only required width |
| Can set width & height | Width & height do not work normally |
| Example: div, p | Example: span, a |

---

## 5. Using CSS to Change Behavior

We can change element type using the `display` property.

### Make Block Element Inline

```css
div {
  display: inline;
}
```

### Make Inline Element Block

```css
span {
  display: block;
}
```

---

## 6. Conclusion

Block and inline elements behave differently in HTML.

Block elements:
- Start on new line  
- Take full width  

Inline elements:
- Stay in same line  
- Take only required space  
