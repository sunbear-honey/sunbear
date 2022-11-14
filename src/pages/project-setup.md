---
layout: ../layouts/MarkdownLayout.astro
---

# project-setup

A template to set up a basic project quickly.

```html
<div class="app">
  <header>
    <h1>Project Template</h1>
  </header>
  <main>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis dolorem voluptates laboriosam veritatis explicabo dignissimos incidunt! Necessitatibus quam eum, deleniti quaerat voluptate dolore quisquam velit, sit debitis, placeat at repellat.
    </p>
  </main>
  <footer>
    <p>
      SunbearDay Project Template (2022)
    </p>
  </footer>
</div>
```

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');

:root {
  --font-size-base: calc(16 / 16);
  --font-size-desktop: calc(20 / 16);
  --font-size-900: calc(var(--font-size-base) * 4.209em);
  --font-size-800: calc(var(--font-size-base) * 3.157em);
  --font-size-700: calc(var(--font-size-base) * 2.369em);
  --font-size-600: calc(var(--font-size-base) * 1.777em);
  --font-size-500: calc(var(--font-size-base) * 1.333em);
  --font-size-400: calc(var(--font-size-base) * 1em);
  --font-size-300: calc(var(--font-size-base) * 0.75em);
  --font-size-200: calc(var(--font-size-base) * 0.563em);
  --font-size-100: calc(var(--font-size-base) * 0.422em);

  --font-family: 'Inter', sans-serif;
}


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
  font-family: var(--font-family);
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

:is(h1, h2, h3, h4, h5, h6) {
  font-weight: 700;
}

h1 {
  font-size: var(--font-size-700);
}

h2 {
  font-size: var(--font-size-600);
}

h3 {
  font-size: var(--font-size-500);
}

h4 {
  font-size: var(--font-size-400);
}

h5 {
  font-size: var(--font-size-300);
}

h6 {
  font-size: var(--font-size-200);
}

p {
  font-size: var(--font-size-400);
}

@media (min-width: 37.5rem) {
  :root {
    --font-size-base: var(--font-size-desktop);
  }
}

.app {
  height: 100%;
  margin-inline: auto;
  max-width: 65ch;
  padding: 1em;
}

main {
  height: 100%;
}

footer {
  padding-block: 2em;
  text-align: center;
}
```