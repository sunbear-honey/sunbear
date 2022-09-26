---
layout: ../layouts/MarkdownLayout.astro
title: "CSS Reset"
---

# CSS Reset

```css
/* ./styles/reset.css */

/* 
Thanks to Josh Comeau for the modern simple reset.
  https://www.joshwcomeau.com/css/custom-css-reset/
*/

:is(*, *::before, *::after) {
  box-sizing: border-box;
}

* {
  margin: 0;
}

:is(html, body) {
  height: 100%;
}

body {
  line-height: 1.5;
}

img, picture, video, canvas, svg {
  display: block;
  max-width: 100%;
}

:is(input, button, textarea, select) {
  font: inherit;
}

:is(p, h1, h2, h3, h4, h5, h6) {
  overflow-wrap: break-word;
}
```
