# First Visit: The Safety Sweep

A self-contained first-person home-assessment activity for in-home caregiver training.
The learner walks a client's apartment on an initial visit and inspects fifteen things
worth noticing — entry, corridor, bathroom, toilet room, both bedrooms, kitchen and living room.

Every finding also carries a **scope decision**: is it yours to **fix now**, yours to **ask
about first**, or yours to **report**? Noticing a hazard is the easy half. Doing more than your
role allows is as much a mistake as doing nothing. The split is deliberately uneven —
5 fix, 4 ask, 6 report — so the pattern can't be guessed.

Module: Mobility & Safety. Primary outcome: identifying and reducing home safety risks.

## Controls

**Desktop** — WASD or arrow keys to walk, mouse to look (click the scene to capture the
pointer, Esc to release), `E` or click to inspect a nearby hotspot.

**Phone and tablet** — an arrow pad to walk, turn buttons to look around, and an Inspect
button that appears when you're close to something. Drag anywhere to look.

The **On-screen controls** button in the top bar forces the touch controls on at any
window size, so the mobile experience can be reviewed from a desktop.

## Technical

- Single HTML file, ~7.4 MB, **no external requests of any kind** — works offline from disk.
- Three.js, GLTFLoader and three-mesh-bvh inlined; the apartment model embedded as base64.
- BVH-accelerated collision, two-height wall probing, axis-separated steps for wall sliding.
- Movement is clamped to the model's own footprint, so the player cannot leave the apartment.

## Credits

Apartment model: [Appartement](https://sketchfab.com/3d-models/appartement-6a7a5fe208344b2e8123a88923dbd5b3)
by [SrMonteiro](https://sketchfab.com/crispimrafael) on Sketchfab, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

## Caveat

General training content. Not a substitute for your agency's assessment form, its policies,
or the client's care plan. The fix / ask / report calls reflect a typical non-licensed
caregiver scope and should be reconciled with local policy.
