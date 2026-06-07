# Squarespace Embed Instructions

## iframe snippets

In the Squarespace page editor, add a **Code Block** and paste the relevant snippet.

**Demo 1 — Green's Function Explorer**
```html
<iframe
  src="https://colej.github.io/pde-examples/pages/01_green_explorer.html"
  width="100%" height="480" frameborder="0" scrolling="no"
  style="border:none;max-width:620px;display:block;margin:0 auto;">
</iframe>
```

**Demo 2 — Poisson Solver**
```html
<iframe
  src="https://colej.github.io/pde-examples/pages/02_poisson_solver.html"
  width="100%" height="480" frameborder="0" scrolling="no"
  style="border:none;max-width:620px;display:block;margin:0 auto;">
</iframe>
```

**Demo 3 — Neural Operator**
```html
<iframe
  src="https://colej.github.io/pde-examples/pages/03_neural_operator.html"
  width="100%" height="640" frameborder="0" scrolling="no"
  style="border:none;max-width:640px;display:block;margin:0 auto;">
</iframe>
```

## If Squarespace strips the iframe tag

Go to **Settings → Advanced → Code Injection**, select the relevant page, and paste the snippet into the **Page Header** or **Footer** field instead of a Code Block.

## Notes

- Demo 3 requires internet access to load TensorFlow.js from CDN (~1.5 MB, cached after first load).
- All demos support touch — mobile visitors can interact normally.
- The `max-width` in each snippet keeps the demos centred on wide Squarespace layouts.
- Heights can be adjusted: 480px suits Demos 1 and 2; 640px gives Demo 3 enough room to show all result panels after training.
