# Light Spot Planner

A 2D/3D planner for light spots, shadows and daylight. Lay out rooms, furniture and fixtures, set beam angles and mounting heights, and see how the light falls — including shadows cast by walls and furniture, and natural light coming through windows.

**Live demo:** https://meduzkin.github.io/light-planner/

Single HTML file, no build step. 3D powered by [Three.js](https://threejs.org/) (CDN). UI in English/Russian, everything auto-saves to the browser (localStorage) — nothing is lost on refresh.

## Features

**2D plan (top view):**
- draw walls as segments (arbitrary shapes, multiple rooms);
- windows and doors as openings that slide along walls and snap between them;
- furniture / objects (boxes with height, wall-mount offset and rotation);
- fixtures: spot, linear (LED strip by count or pitch), panel, chandelier (omni cluster), wall sconce;
- power in watts per fixture; tracks (rails) with attached, distributable fixtures;
- beam / field angles, tilt, azimuth, up/down facing.

**3D view (visualizer):**
- real lights with shadows — solid walls block light, it only passes through window/door openings;
- daylight: a draggable sun point, window light patch + soft fill from the opening, sky light;
- detail switch (schematic / medium / realistic) to trade quality for speed in realtime;
- orbit camera, gizmo dragging, click-to-select; add/edit objects, lights and the sun right in 3D.

**Editing:**
- Photoshop-style layer tree (collapsible groups, per-layer visibility, pin objects to layers);
- copy / paste / duplicate any object (Ctrl/Cmd + C / V / D);
- import / export the whole scene to a JSON file.

## Controls

- **2D:** click — select, drag — move, RMB/Space — pan, wheel — zoom. Drawing walls: click — point (0.1 m snap, Shift — free, snaps to wall ends), double-click / Esc — finish.
- **3D:** click — select, gizmo — move, drag window/sun with the mouse, LMB on background — orbit, wheel — zoom.

## Hosting

Static site on GitHub Pages. Entry point is `index.html`.

🤖 Built with [Claude Code](https://claude.com/claude-code)
