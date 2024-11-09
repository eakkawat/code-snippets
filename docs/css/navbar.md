# Navbar

## Navbar structure

The basic navbar structure is as follows:

```Folder structure
<header>
  |--<nav>
       |--<ul>
           |--<li>
                |--<a>
```

### Navbar example

```HTML
  <header>
    <nav>
      <a href="#" class="logo">Logo</a>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>
```

```CSS
  header {
    background-color: #333;
    padding: 10px;
  }

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
```

::: tip
How to add logo in navbar?

1. Add `<a>` tag inside `<nav>` tag.
2. Add `class="logo"` to `<a>` tag.
3. Add `logo` class in CSS.
4. In .logo class, add `backgroud-image: url('path-to-image');` property.
   :::
