# Centering content

## Centering itself

To center an element horizontally within its parent, you can use the following code:

```HTML
<div class="container"></div>
```

```CSS
  .container {
    max-width: 1000px;
    margin: 0 auto;
  }
```

### Explanation

- The `margin: 0 auto;` property centers the element horizontally within its parent.
- The `auto` value calculates the remaining space on the left and right sides of the element and applies it as margin, effectively centering the element.

::: warning
`max-width: 1000px;` property ensures that the element does not take up the full width of the viewport. Without max-width, the element will stretch to fill the entire width
:::

::: warning
This method only works for block elements. If you want to center an inline element, you can use `text-align: center;` on its parent element.
:::

## Flexbox centering

flexbox is a great way to center content. To center children elements horizontally and vertically, you can use the following code:

```HTML
<div class="container">
  <div class="content"></div>
</div>
```

```CSS {4-5}
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

```

### Explanation

In `flex-direction: row;` context (which is the default value),

- `justify-content: center;` centers the children elements horizontally.
- `align-items: center;` centers the children elements vertically.

## Grid centering

Similar to flexbox, you can use grid to center content but this time you use `display: grid`. To center children elements horizontally and vertically, you can use the following code:

```HTML
<div class="container">
  <div class="content"></div>
</div>
```

```CSS {3-4}
.container {
  display: grid;
  justify-content: center;
  align-content: center;
}
```

## Transform centering

This method uses the `transform` property to center an element. The parent elment must have a `position: relative;` property, and the child element must have a `position: absolute;` property. Then offset the child element by `top: 50%;` and `left: 50%;` and use `transform: translate(-50%, -50%);` to center it.

```HTML
<div class="container">
  <div class="content"></div>
</div>
```

```CSS
.container {
  position: relative;
}

.content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```
