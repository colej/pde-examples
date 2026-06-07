# pde-examples

Interactive browser demos exploring Green's functions and neural operators for the 1D Poisson equation. No build step, no server — pure HTML and JavaScript.

## Demos

| File | What it shows |
|------|---------------|
| `pages/01_green_explorer.html` | Interactive G(x,y) heatmap — hover to see the impulse response at any y₀ |
| `pages/02_poisson_solver.html` | Draw f(x) with the mouse; u(x) = ∫G f dy updates in real time |
| `pages/03_neural_operator.html` | Trains a DeepONet in the browser; compares the learned kernel to the true G |

## Structure

```
pde-examples/
├── index.html              ← landing page (GitHub Pages root)
├── pages/
│   ├── 01_green_explorer.html
│   ├── 02_poisson_solver.html
│   └── 03_neural_operator.html
├── README.md
└── SQUARESPACE.md          ← iframe embed instructions
```

## Dependencies

- Demos 1 & 2: none — pure JavaScript
- Demo 3: [TensorFlow.js 4.17](https://cdn.jsdelivr.net/npm/@tensorflow/tfjs@4.17.0/) loaded from CDN at runtime

## Embedding

See [`SQUARESPACE.md`](./SQUARESPACE.md) for iframe snippets and Squarespace-specific instructions.
