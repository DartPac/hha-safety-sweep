# H5P activities — Mobility & Safety / First Visit: The Safety Sweep

Three `.h5p` packages that pair with the walkthrough at
https://dartpac.github.io/hha-safety-sweep/

| File | Content type | What it assesses |
|---|---|---|
| `safety-sweep-mark-the-words.h5p` | H5P.MarkTheWords 1.11 | Spotting out-of-scope actions in a written visit note (LO1 / LO11) |
| `safety-sweep-fix-ask-report.h5p` | H5P.DragQuestion 1.15 | Sorting 9 findings into fix / ask / report (LO4 + LO1) |
| `safety-sweep-kitchen-hotspot.h5p` | H5P.ImageHotspotQuestion 1.8 | Knowing where forgotten cooking shows first (LO4) |

## Important: these are content-only packages

They contain `h5p.json` and `content/` but **no library folders**. They import correctly on any
platform that already has the three content types installed — which is the normal case, since all
three are core H5P Hub types. If an import fails with a missing-library error, install the content
type from the H5P Hub first, then re-import:

- Mark the Words
- Drag and Drop
- Image Hotspot Question

Libraries could not be bundled: H5P ships content-type JavaScript as build artifacts that are not in
the public source repositories, and the H5P Hub API is not reachable from the build environment.

## Not yet verified in a running H5P instance

Each package has been checked structurally against the official `semantics.json` for its content type
(all required fields present and correctly typed, referenced assets present in the archive). None has
been opened in a real H5P player, because the libraries needed to run one are not available here.

**Import `safety-sweep-mark-the-words.h5p` first** — it has the simplest structure, so if something is
wrong with the approach it will surface there fastest and cheapest.

The one most likely to need adjustment is the drag-and-drop: element and drop-zone positions are
percentages I calculated rather than placed by eye, so spacing may want nudging in the H5P editor.
Content is correct; only the layout is unverified.

## Answer keys

**Mark the Words** — four correct marks: `refilled` (filling a pill organiser is medication
administration), `turned` (adjusting a water heater), `removed` (taking up the client's rug without
asking), `reassured` (offering a clinical opinion about dizziness).

**Fix / Ask / Report** — Fix: curled mat, extension cord, missing night light. Ask: lifting rug edge,
coffee table in the route, deep sofa. Report: no grab bar, water above 120°F, low toilet.

**Kitchen hotspot** — correct answer is the gas hob. Every wrong option has its own feedback
explaining why it matters but is not the answer.

## Image credit

The kitchen still is rendered from the apartment model used in the walkthrough:
[Appartement](https://sketchfab.com/3d-models/appartement-6a7a5fe208344b2e8123a88923dbd5b3) by
[SrMonteiro](https://sketchfab.com/crispimrafael), CC BY 4.0. Attribution carries to any reuse.

## A note on "spot the hazard"

The original plan was a find-the-hazard activity on room stills. The apartment model is a clean
showroom interior — there is no curling rug, trailing cord or clutter modelled in the geometry, so
learners would have been clicking things that are not visibly hazardous. The kitchen question was
reframed to ask where risk *concentrates*, which the image genuinely supports. A true spot-the-hazard
activity needs photographs of a real, lived-in home.
