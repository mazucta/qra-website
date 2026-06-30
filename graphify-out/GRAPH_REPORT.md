# Graph Report - /Users/shyxx/Desktop/projects/sakura-showcase  (2026-07-01)

## Corpus Check
- 24 files · ~108,443 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 25 nodes · 33 edges · 5 communities (4 shown, 1 thin omitted)
- Extraction: 67% EXTRACTED · 33% INFERRED · 0% AMBIGUOUS · INFERRED: 11 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Portfolio Examples & UI|Portfolio Examples & UI]]
- [[_COMMUNITY_3D Rendering Engine|3D Rendering Engine]]
- [[_COMMUNITY_Scroll Scene Timeline|Scroll Scene Timeline]]
- [[_COMMUNITY_Telegram Booking Bot|Telegram Booking Bot]]
- [[_COMMUNITY_Cursor Parallax|Cursor Parallax]]

## God Nodes (most connected - your core abstractions)
1. `3D Sakura Scene` - 9 edges
2. `Scroll-Driven Scene Timeline (tree to molecule)` - 6 edges
3. `Telegram Booking Bot Demo` - 5 edges
4. `Project Viewer Modal (native dialog)` - 4 edges
5. `Beauty Website Demo Site (Lash/Brow/PMU Studio)` - 4 edges
6. `Three.js` - 3 edges
7. `Custom GLSL Vertex/Fragment Shaders` - 3 edges
8. `Stage: Orbit` - 3 edges
9. `Stage: Disintegration` - 3 edges
10. `Hero Portfolio Gallery` - 3 edges

## Surprising Connections (you probably didn't know these)
- `Project Viewer Modal (native dialog)` --references--> `Telegram Booking Bot Demo`  [INFERRED]
  index.html → examples/telegram-bot/index.html
- `QRA Studio Showcase (README)` --references--> `3D Sakura Scene`  [EXTRACTED]
  README.md → index.html
- `Beauty Site Demo (Lash/Brow Landing)` --references--> `3D Sakura Scene`  [EXTRACTED]
  examples/beauty-site/index.html → index.html
- `Beauty Website Demo Site (Lash/Brow/PMU Studio)` --references--> `3D Sakura Scene`  [EXTRACTED]
  examples/beauty-website/index.html → index.html
- `Telegram Booking Bot Demo` --references--> `3D Sakura Scene`  [EXTRACTED]
  examples/telegram-bot/index.html → index.html

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Scroll-Driven 3D Scene Stages** — index_stage_tree, index_stage_orbit, index_stage_disintegration, index_stage_molecule [EXTRACTED 1.00]
- **Portfolio Demo Surfaces in Project Viewer** — index_project_viewer_modal, beauty_website_index_demo_site, beauty_site_index_demo_site, telegram_bot_index_booking_bot [INFERRED 0.85]
- **Telegram Booking Flow** — telegram_bot_index_chat_mockup, telegram_bot_index_calendar_mockup, telegram_bot_index_google_calendar [EXTRACTED 1.00]

## Communities (5 total, 1 thin omitted)

### Community 0 - "Portfolio Examples & UI"
Cohesion: 0.38
Nodes (7): Beauty Site Demo (Lash/Brow Landing), Beauty Website Demo Site (Lash/Brow/PMU Studio), Contact Lead Form, Live Iframe Mini-Previews, Hero Portfolio Gallery, i18n System (RU/EN/ET/DE), Project Viewer Modal (native dialog)

### Community 1 - "3D Rendering Engine"
Cohesion: 0.38
Nodes (7): 3D Sakura Scene, Ambient Falling Petals, Auto Quality Scaling, Custom GLSL Vertex/Fragment Shaders, Three.js, UnrealBloom Postprocessing, QRA Studio Showcase (README)

### Community 2 - "Scroll Scene Timeline"
Cohesion: 0.53
Nodes (6): Lenis Smooth Scroll, Scroll-Driven Scene Timeline (tree to molecule), Stage: Disintegration, Stage: Molecular Lattice, Stage: Orbit, Stage: Sakura Tree

### Community 3 - "Telegram Booking Bot"
Cohesion: 0.67
Nodes (4): Telegram Booking Bot Demo, Calendar + Event Mockup, Telegram Chat Mockup, Google Calendar Integration

## Knowledge Gaps
- **6 isolated node(s):** `QRA Studio Showcase (README)`, `Lenis Smooth Scroll`, `Cursor Parallax`, `Ambient Falling Petals`, `Contact Lead Form` (+1 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `3D Sakura Scene` connect `3D Rendering Engine` to `Portfolio Examples & UI`, `Scroll Scene Timeline`, `Telegram Booking Bot`?**
  _High betweenness centrality (0.664) - this node is a cross-community bridge._
- **Why does `Scroll-Driven Scene Timeline (tree to molecule)` connect `Scroll Scene Timeline` to `3D Rendering Engine`?**
  _High betweenness centrality (0.348) - this node is a cross-community bridge._
- **Why does `Telegram Booking Bot Demo` connect `Telegram Booking Bot` to `Portfolio Examples & UI`, `3D Rendering Engine`?**
  _High betweenness centrality (0.276) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `Project Viewer Modal (native dialog)` (e.g. with `Beauty Site Demo (Lash/Brow Landing)` and `Beauty Website Demo Site (Lash/Brow/PMU Studio)`) actually correct?**
  _`Project Viewer Modal (native dialog)` has 3 INFERRED edges - model-reasoned connections that need verification._
- **Are the 3 inferred relationships involving `Beauty Website Demo Site (Lash/Brow/PMU Studio)` (e.g. with `Beauty Site Demo (Lash/Brow Landing)` and `Live Iframe Mini-Previews`) actually correct?**
  _`Beauty Website Demo Site (Lash/Brow/PMU Studio)` has 3 INFERRED edges - model-reasoned connections that need verification._
- **What connects `QRA Studio Showcase (README)`, `Lenis Smooth Scroll`, `Cursor Parallax` to the rest of the system?**
  _7 weakly-connected nodes found - possible documentation gaps or missing edges._