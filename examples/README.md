# interactive-3d-web-examples — Examples

Interactive, **production-grade** 3D built with Three.js (r160) — no build step, just open the file.

| File | Description |
| --- | --- |
| [`pointer-particles.html`](./pointer-particles.html) | A `BufferGeometry` particle field (up to 9,000 points) that springs back to a home layout while the pointer attracts particles — or repels them while pressed. Additive blending for glow; the live particle count scales with measured performance. |

### Expert / production features (every example)

- **Capability detection + graceful fallback** — probes WebGL2 → WebGL → none. With no WebGL context (or `prefers-reduced-motion`) it paints a tasteful CSS starfield/gradient poster instead of a blank canvas; low-power devices start with a smaller particle budget.
- **Adaptive performance** — DPR capped at 2; a rolling FPS average steps DPR **and the live particle count** down below 50 fps and back up above 58 fps with hysteresis (the spring simulation only integrates the live set, so cost drops with count). The loop pauses when the canvas is offscreen (`IntersectionObserver`) or the tab is hidden.
- **Strict cleanup** — one teardown on `pagehide` removes every pointer/resize listener, cancels rAF, and disposes the geometry, material and renderer.
- **Accessibility** — the canvas is `role="img"` with an `aria-label`; the optional FPS/quality readout is a real keyboard-focusable `<button>` with a visible focus ring; motion respects `prefers-reduced-motion` (calm static field, no interaction loop).
- **Premium look** — ACES Filmic tone mapping and an indigo→cyan radial hue ramp with additive glow.

Three.js r160 is loaded as ES modules through an importmap on **jsDelivr only** (`three` + `three/addons/`). The pointer is projected onto the `z = 0` plane with a `Raycaster`, and particles integrate a damped spring toward their rest positions.

Part of AETumi's interactive 3D examples hub: https://aetumi.app/interactive
