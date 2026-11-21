# Rokas Sileikis

Full-stack engineer in Zürich, working on regulated medical software. React and TypeScript, Laravel, Rust and Tauri. English and German.

### collab-canvas

A multiplayer whiteboard: everyone on the same room link draws together and sees the others' cursors and unfinished strokes live.
The board is a Yjs document, synced through a Cloudflare Worker with one SQLite-backed Durable Object per room. Updates are appended as rows and compacted into snapshots stored in 1 MB parts; a failed write aborts the room instead of dropping strokes quietly. No automated tests yet, only type-check and lint.

[Open a room](https://collab-canvas.rokass.org) · [Code](https://github.com/rokas-th/collab-canvas)

### memory-globe

A 3D globe of places I have travelled, with a photo gallery for each city, in React Three Fiber.
The Earth texture loads in tiers, up to 16K on desktop GPUs that can hold it. The build reads the image headers and fails if a gallery entry and its file disagree, so a bad content edit stops the deploy.

[Open the globe](https://memory-globe.rokass.org)

I also build websites for small businesses. More at [rokass.org](https://rokass.org).
