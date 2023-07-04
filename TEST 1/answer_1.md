# Question 1. Explain all the CSS positions(static, fixed, sticky, relative, absolute) with one code example each

## ◻ Static Position

The default positioning property is static, which means elements are displayed in their normal order as they appear in the HTML markup. Elements with static positioning are not affected by other positioning properties or offsets.

```
<!DOCTYPE html>
<html>
  <head>
    <style>
      .box {
        width: 150px;
        height: 150px;
        background-color: #ff6384;
      }
    </style>
  </head>
  <body>
    <div class="box"></div>
  </body>
</html>
```

---

## ◻ Fixed Position

Elements with a fixed position are positioned relative to the browser window and do not move when the page is scrolled. This can be useful for creating persistent navigation bars or other elements that should remain visible at all times.

```
<!DOCTYPE html>
<html>
  <head>
    <style>
      .box {
        width: 150px;
        height: 150px;
        background-color: #ff9f40;
        position: fixed;
        top: 20px;
        left: 20px;
      }
    </style>
  </head>
  <body>
    <div class="box"></div>
  </body>
</html>

```

---

## ◻ Sticky Position

The sticky position combines elements of both relative and fixed positions. It behaves as relative until the specified threshold is met, after which it acts as fixed. Sticky elements are useful for creating elements that stick to the top or bottom of the viewport as the user scrolls.

```
<!DOCTYPE html>
<html>
  <head>
    <style>
      .box {
        width: 150px;
        height: 150px;
        background-color: #ffd740;
        position: sticky;
        top: 50px;
      }
    </style>
  </head>
  <body>
    <div class="box"></div>
    <div style="height: 2000px;"></div>
  </body>
</html>
```

---

## ◻ Relative Positioning

Elements with relative positioning are positioned relative to their normal position. They can be moved around using the top, bottom, left, and right properties. However, their new positions do not affect other elements on the page.

```
<!DOCTYPE html>
<html>
  <head>
    <style>
      .box {
        width: 150px;
        height: 150px;
        background-color: #40ffbf;
        position: relative;
        top: 20px;
        left: 20px;
      }
    </style>
  </head>
  <body>
    <div class="box"></div>
  </body>
</html>
```

---

## ◻ Absolute Positioning

Elements with absolute positioning are positioned relative to their nearest positioned ancestor. If no positioned ancestor is found, they are positioned relative to the initial containing block, which is usually the browser window. Absolute positioning allows precise control over an element's position and is commonly used for overlays or tooltips.

```
<!DOCTYPE html>
<html>
  <head>
    <style>
      .container {
        position: relative;
        width: 400px;
        height: 400px;
      }

      .box {
        width: 150px;
        height: 150px;
        background-color: #ff40a6;
        position: absolute;
        top: 50px;
        left: 50px;
      }
    </style>

  </head>
  <body>
    <div class="container">
      <div class="box"></div>
    </div>
  </body>
</html>
```
