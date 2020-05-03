# Learning BS4

## 2. Navbar Concepts

https://www.youtube.com/watch?v=23bpce-5s8I&list=PL55RiY5tL51rLqH4-8LBVlUTIFF70dxhb&index=3

Navbars as `<nav>` elements need a `navbar` class

- Add additional brand modifiers like `navbar-light` and `bg-light` to give it a theme
- Adding a class like `mr-auto` (margin-right: auto) will cause a given nav to float to the left

Inside the navbar:

- Inside the navbar, add `a` with `navbar-brand` to position a brand link at top-left
- Menu items go in a `ul` with `navbar-nav`
  - items should be `li`'s with `nav-item`, containing `a`'s with `nav-link`
  - You will probably want navs to be inline, not stacked (default, because mobile-first)
    - Fix this by wrapping the menu (`ul`) in a `div` with `collapse navbar-collapse`
    - You will also need to add a `navbar-expand` class to the `nav` element to show this
      - Note- this can also accept a responsive breakpoint to only expand the nav at certain sizes- e.g., `navbar-expand-sm`
      - This will also push the nav menu (by default) back to the left- fix with `ml-auto` on the `ul` (will push it back to the right)

Adding a toggle

- Before the `div.navbar-collapse`, add a `button.navbar-toggler` containing `span.navbar-toggler-icon`. 
- The `button` also needs a `data-toggle="collapse"` and `data-target="#navbarMenu"` (or whatever the ID of the navbar is) to actually work
- Finally, add the specified ID (e.g., `id="navbarMenu"` to the `div.navbar-collapse`)
