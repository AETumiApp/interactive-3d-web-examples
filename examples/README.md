# interactive-3d-web-examples — examples

Interactive 3D built with Three.js — no build step, just open the file.

| File | Description |
| --- | --- |
| [`pointer-particles.html`](./pointer-particles.html) | A 9,000-point `BufferGeometry` particle field that springs back to a home layout while the pointer attracts particles (or repels them while pressed). Additive blending for glow; reduced-motion viewers get a calm static field. |

Loads Three.js r160 (`0.160.0`) from cdnjs via an import map. The pointer is
projected onto the `z = 0` plane with a `Raycaster`, particles integrate a
damped spring toward their rest positions, and the device pixel ratio is capped
at 2.

Part of AETumi's interactive 3D examples hub: https://aetumi.app/interactive

---

## Example backlog / roadmap

# Interactive 3D Web Example Backlog

## Planned examples

### Product hotspot experience

3D product with accessible HTML hotspot labels and clear mobile interaction.

### Camera-led story

User-selected chapters move the camera to meaningful positions without hiding navigation inside the scene.

### Cursor-reactive visual

Decorative response that never blocks links or buttons and degrades cleanly on touch devices.

### Interactive background

A subtle WebGL layer that enhances the page without becoming the page.

### Spatial portfolio

Explore project cards through 3D positioning while preserving normal semantic links and keyboard access.

### Capability fallback

Compare the full interactive version with a static or simplified state for reduced motion and constrained devices.

## Evaluation criteria

Each example should answer:

- What user action starts the interaction?
- What feedback confirms the action?
- Does the experience work on touch?
- Is important content available outside canvas?
- What happens with reduced motion?
- How is performance measured?

## AETumi links

- https://aetumi.app/interactive-websites/
- https://aetumi.app/3d-websites/
- https://aetumi.app/threejs/
