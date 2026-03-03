# Technical Paper on CSS Positioning: Relative and Absolute

## 1. Introduction

CSS positioning is used to control the location of elements on a web page.

The `position` property has different values.  
In this paper, we will study:

- relative  
- absolute  

---

## 2. position: relative

When we use `position: relative;`, the element moves from its normal position.

Important points:

- The element keeps its original space.
- It moves based on top, bottom, left, and right.
- Other elements are not affected.

### Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
.box {
  width: 200px;
  height: 100px;
  background-color: lightblue;
  position: relative;
  top: 20px;
  left: 30px;
}
</style>
</head>
<body>

<div class="box">
  Relative Box
</div>

</body>
</html>
```

In this example:
- The box moves 20px down.
- The box moves 30px right.
- But its original space is still reserved.

---

## 3. position: absolute

When we use `position: absolute;`, the element is removed from normal flow.

Important points:

- It does not keep its original space.
- It is positioned relative to the nearest positioned parent.
- If no positioned parent exists, it uses the body.

### Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
.parent {
  position: relative;
  width: 300px;
  height: 200px;
  background-color: lightgray;
}

.child {
  position: absolute;
  top: 20px;
  right: 20px;
  width: 100px;
  height: 50px;
  background-color: lightcoral;
}
</style>
</head>
<body>

<div class="parent">
  <div class="child">
    Absolute Box
  </div>
</div>

</body>
</html>
```

In this example:
- The child moves inside the parent.
- It is placed 20px from top and 20px from right.
- It does not take normal space.

---

## 4. Difference Between Relative and Absolute

| Relative | Absolute |
|-----------|-----------|
| Keeps original space | Removes from normal flow |
| Moves from its own position | Moves relative to parent |
| Used for small adjustments | Used for exact positioning |

---

## 5. Conclusion

`position: relative` moves an element from its normal place but keeps its space.

`position: absolute` removes the element from normal flow and places it exactly where needed.
