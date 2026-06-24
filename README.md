# VELA — sakura showcase

Single-file agency showcase. Scroll-driven 3D sakura (thick curved trunk, dense
pink-to-rose dome canopy) that disintegrates into a glowing molecular lattice as
you scroll, then hands off to content sections.

- **Stack:** Three.js + custom GLSL shaders, UnrealBloom post-processing, Lenis smooth scroll — all via CDN, no build step.
- **Languages:** RU · EN · ET · DE (switcher top-right, persisted in `localStorage`).
- **Sections:** hero → capabilities → "to atoms" → molecule → Services → Process → Contact.

## Run

Just open `index.html`, or serve the folder:

```bash
python3 -m http.server 4599
# http://localhost:4599
```

## Customise

- Brand name / copy: edit the `I18N` dictionary in `index.html`.
- Contact email: replace `hello@vela.studio`.
- Tree shape: `spine` control points and the `CANOPY` / `RX,RY,RZ` constants.
- Glow: `UnrealBloomPass` params and the petal `glow` value.
