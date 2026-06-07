# PDE Interactive Demos — Squarespace Embed Guide

Three self-contained JavaScript demos, no backend required.

| File | Description |
|------|-------------|
| `01_green_explorer.html` | Hover over G(x,y) heatmap; see the impulse response |
| `02_poisson_solver.html` | Draw f(x) with mouse; u(x) updates live |
| `03_neural_operator.html` | Trains a DeepONet in the browser (~20s); compares learned vs true kernel |

---

## Step 1 — Host on GitHub Pages (free, ~2 min)

1. Create a new public GitHub repo, e.g. **`pde-demos`**
2. Upload the three HTML files to the repo root
3. Go to **Settings → Pages → Source → Deploy from branch → `main` → `/ (root)` → Save**
4. Wait ~60 seconds; your pages will be live at:
   ```
   https://YOUR-USERNAME.github.io/pde-demos/01_green_explorer.html
   https://YOUR-USERNAME.github.io/pde-demos/02_poisson_solver.html
   https://YOUR-USERNAME.github.io/pde-demos/03_neural_operator.html
   ```

---

## Step 2 — Embed in Squarespace

In the Squarespace page editor:

1. Click **+** to add a block → choose **Code**
2. Paste the iframe snippet for whichever demo you want, substituting your GitHub username

**Demo 1 — Green's Function Explorer**
```html
<iframe
  src="https://YOUR-USERNAME.github.io/pde-demos/01_green_explorer.html"
  width="100%" height="480" frameborder="0" scrolling="no"
  style="border:none;max-width:620px;display:block;margin:0 auto;">
</iframe>
```

**Demo 2 — Poisson Solver**
```html
<iframe
  src="https://YOUR-USERNAME.github.io/pde-demos/02_poisson_solver.html"
  width="100%" height="480" frameborder="0" scrolling="no"
  style="border:none;max-width:620px;display:block;margin:0 auto;">
</iframe>
```

**Demo 3 — Neural Operator**
```html
<iframe
  src="https://YOUR-USERNAME.github.io/pde-demos/03_neural_operator.html"
  width="100%" height="640" frameborder="0" scrolling="no"
  style="border:none;max-width:640px;display:block;margin:0 auto;">
</iframe>
```

---

## Notes

- **Demo 1 & 2** have zero external dependencies — pure JavaScript.
- **Demo 3** loads TensorFlow.js (~1.5 MB) from jsDelivr CDN on first visit.
- All demos are responsive; the `max-width` in the iframe style keeps them readable on wide screens.
- If Squarespace strips the `<iframe>` tag, go to **Settings → Advanced → Code Injection** and add it to the page footer instead.
- Touch/mobile is supported on all three demos.
