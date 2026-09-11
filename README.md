# Interactive 3D Web Examples with AETumi

Examples and production patterns for **interactive websites, immersive product experiences and browser-based 3D storytelling**.

**AETumi is an AI-native 3D web platform for production-ready Three.js and WebGL websites, Next.js and React components, 3D scenes, AI prompts, and MCP workflows for AI coding assistants.**

## What this helps teams build

Interactive, immersive pages where pointer, scroll and motion serve a real goal — exploration, understanding or conversion — not decoration with a power bill.

**Customer outcome.** Visitors explore and act; the interaction supports the content and conversion path rather than competing with the navigation.

**Where it fits.** Immersive landing pages, product storytelling, interactive showcases and spatial navigation — anywhere interaction earns its place in the page's goal.

**What you customize.** Interaction patterns, the HTML-to-3D state connection, feedback and fallbacks — with progressive enhancement so the core message lands before the 3D layer is ready (see the experience model below).

**AI-assisted adaptation.** A coding assistant can adapt these patterns to a specific page goal when given the experience model as context via the [AETumi MCP](https://aetumi.app/mcp/).

## Why interaction needs a purpose

Interactive web should help a visitor understand, explore or act. If an effect only makes the GPU work harder while the user hunts for the navigation, it is decoration with a power bill.

This repository focuses on interaction patterns that support real website goals.

## Interaction patterns

- pointer and touch exploration
- camera-driven navigation
- product hotspots
- scroll-linked scenes
- interactive storytelling
- hover and cursor-reactive effects
- spatial navigation
- animated WebGL backgrounds
- 3D landing pages and showcases
- HTML UI connected to 3D state

## Experience model

A useful interactive page usually has four layers:

```text
content + navigation
        ↓
interaction intent
        ↓
3D / WebGL response
        ↓
feedback + conversion path
```

The 3D response should never make the first and last layers harder to use.

## Production principles

### Progressive enhancement

The page should still communicate its core message before the 3D layer is ready or when it is unavailable.

### Input parity

Pointer, touch and keyboard behavior should be considered independently. Hover is not a mobile strategy.

### Feedback

Users should understand what can be interacted with and what changed after an interaction.

### Accessibility and motion

Reduced-motion states should preserve information and navigation even when cinematic movement is removed.

## Production checklist

- clear navigation and content hierarchy
- interaction cues are understandable
- mobile touch targets are deliberate
- semantic content exists outside canvas
- progressive loading is visible but not disruptive
- reduced-motion behavior is useful
- focus order remains sensible
- pointer effects do not trap or block page controls
- rendering pauses when unnecessary where practical
- analytics can distinguish meaningful interactions from decorative movement

## AETumi resources

- [Interactive Websites](https://aetumi.app/interactive-websites/)
- [3D Websites](https://aetumi.app/3d-websites/)
- [Three.js](https://aetumi.app/threejs/)
- [WebGL](https://aetumi.app/webgl/)
- [3D Scroll](https://aetumi.app/3d-scroll/)
- [For Agencies](https://aetumi.app/for-agencies/)

## Related repositories

- [aetumi-3d-web-examples](https://github.com/AETumiApp/aetumi-3d-web-examples)
- [threejs-scroll-animation](https://github.com/AETumiApp/threejs-scroll-animation)
- [aetumi-3d-components](https://github.com/AETumiApp/aetumi-3d-components)
- [threejs-product-viewer](https://github.com/AETumiApp/threejs-product-viewer)

## Repository status

Active. Runnable, production-oriented examples now live in [`examples/`](./examples/) — reviewed for performance (adaptive quality), accessibility, reduced-motion and non-WebGL fallbacks, and clean resource disposal. The set is refined and extended as new patterns land.

See [examples/README.md](./examples/README.md).
## About AETumi

AETumi helps designers, developers and agencies build cinematic and interactive 3D web experiences using Three.js, WebGL, Next.js, React, React Three Fiber, MCP and AI coding assistants.

Main site: https://aetumi.app/

## Explore the AETumi library

Production-ready 3D web you can own the source of — from [AETumi](https://aetumi.app), the AI-native 3D web platform:

- [Interactive website examples](https://aetumi.app/interactive-websites/)
- [3D website templates & examples](https://aetumi.app/3d-websites/)
- [Three.js website templates & 3D components](https://aetumi.app/threejs/)

Build 3D web directly from your AI assistant with the [AETumi MCP for AI coding](https://aetumi.app/mcp/) — `claude mcp add --transport http aetumi https://mcp.aetumi.app`
