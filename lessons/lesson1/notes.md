# Learning BS4

## 1. HOW DO I GRID
 https://www.youtube.com/watch?v=qmPmwdshCMw&list=PL55RiY5tL51rLqH4-8LBVlUTIFF70dxhb&index=2

- Start with container or container-fluid as topmost element inside body
- div with just a class of "col" will be evenly-spaced
- grid is still 12 columns
- responsive classes are not totally needed- col-4 and col-8 are valid
- still can use responsive column modifiers (-md, lg, xl, sm, xs)
- Flexbox-related classes can be applied to elements
  - e.g., justify-content-center (on a row- doesn't work on a column)
  - "justify": main axis. "align"- cross
  - justify-content-(start, end, around, between) are also available
- Vertical alignment:
  - align-items-(start, end, center, stretch, etc.)- stretch is default
- In flexbox, "-content" modifiers relevant for rows, "self" relevant for columns
  - e.g., "align-self-start" on a column will align column to top of the row it sits in, and not fill the height of the row (if the row has height)
- Reordering columns manually- add "order-{n}" class
  - Also possible to make responsive: "order-md-2"
- Offset and push classes are still available, and responsive

