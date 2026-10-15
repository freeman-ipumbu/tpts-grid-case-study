# Desert Signal design system

Desert Signal is the public design direction for TPTS Grid: a map-native digital product with the confidence of financial infrastructure and the sensory character of Namibia.

This is a rationale and token reference, not a distributable copy of the production interface or logo artwork.

## Brand idea

**Movement converges into possibility.**

The mark is imagined as route lines meeting at signal nodes: road, place, payment and people becoming one coherent grid. It avoids literal animals, flags and predictable dune silhouettes. The result should feel Namibian through material, light, scale and rhythm—not decoration.

## Voice

Grid speaks clearly and with local confidence.

| Principle | Use | Avoid |
| --- | --- | --- |
| Direct | “Build my route” | “Leverage our itinerary optimisation solution” |
| Honest | “Application received · verification required” | “You’re live!” before review |
| Grounded | “Namibia moves through here.” | Generic luxury-travel superlatives |
| Useful | Explain what changed and why | Mysterious “AI magic” |
| Warm | “Go further. Book closer.” | Institutional payment language in the travel flow |

Primary lines:

- **Namibia moves through here.**
- **Book the road, not just the room.**
- **Go further. Book closer.**
- **Built on Namibian ground.**

## Colour

| Token | Value | Role |
| --- | --- | --- |
| Night 1000 | `#041617` | Deepest map and editorial ground |
| Night 950 | `#061B1C` | Primary dark surface |
| Night 900 | `#0A292B` | Raised dark surface |
| Atlantic 700 | `#0D6872` | Geographic and interactive depth |
| Atlantic 500 | `#15949A` | Supporting information |
| Signal 400 | `#42D5BD` | Primary action, focus and live signal |
| Signal 300 | `#78EAD4` | Hover and luminous accent |
| Dune 700 | `#A94F32` | Earth-tone emphasis on light surfaces |
| Dune 500 | `#CE6842` | Brand warmth and route accent |
| Sun 400 | `#F1AE3F` | Sparse highlight or caution |
| Salt 50 | `#FFFDF7` | Primary light surface |
| Salt 100 | `#F5EFE2` | Warm secondary surface |
| Limestone 200 | `#DED2BC` | Dividers and landscape-neutral detail |
| Fog 200 | `#BFD2CF` | Quiet information on dark surfaces |
| Lichen 500 | `#53635E` | Accessible secondary copy on light surfaces |

Colour is semantic, never the only carrier of state. Signal teal means action, focus or connection; dune marks editorial warmth and route character; sun is intentionally rare.

## Typography

- **Display:** [Geologica](https://github.com/googlefonts/geologica) — variable, compact and geological without becoming themed.
- **Interface:** [IBM Plex Sans](https://github.com/IBM/plex) — highly legible controls and longer UI copy.
- **Data:** IBM Plex Mono — coordinates, status labels, route metadata and compact system information.

Large display type uses tight tracking and disciplined line breaks. The mono face is a functional layer, not an aesthetic applied to paragraphs.

## Shape and layout

- compact radii (typically 4–12 px) keep the interface infrastructural;
- strong vertical sections make scroll position legible;
- editorial asymmetry creates surprise without disturbing task flows;
- thin lines and small data labels add precision;
- map, imagery and copy overlap only when contrast and pointer behaviour remain unambiguous;
- controls meet a 44 px minimum target, with 48 px preferred for primary actions.

## Motion

Motion should feel like a vehicle settling onto a road: quick, weighted and purposeful.

- entrance motion uses restrained vertical reveal;
- selections have a short spring response;
- the convergence mark can draw its routes and then resolve its nodes;
- scroll navigation announces spatial movement without hijacking scroll;
- loading language may sequence “mapping / connecting / opening Namibia” while work is real;
- every non-essential animation has a reduced-motion equivalent.

Do not use endless parallax, decorative cursor trails, forced scroll sequences or animation that delays access to content.

## Map language

The base map is context; the TPTS overlay is meaning.

- destination anchors are visually distinct from live properties;
- a planned route uses a strong continuous signal, while suggestions can use a lighter or dashed treatment;
- attribution remains visible;
- selected markers provide a corresponding text label and detail surface;
- zoom controls are keyboard operable;
- loading, degraded and unavailable states are written in plain language;
- a directory/list view remains usable without the map.

## Imagery

Imagery should reveal Namibia's scale, texture and transitions: Atlantic fog, salt, basalt, road, dune and human-made shelter. Prefer real, location-accurate photography with rights and provenance over generic safari imagery.

When generative imagery is used for concept presentation, label it, keep it free of false property claims and never present an invented accommodation as bookable inventory.

## Accessibility contract

The visual identity is successful only if the product remains operable:

- preserve visible `:focus-visible` treatment in Signal 400;
- validate text and control contrast in every theme;
- provide meaningful labels for icon-only controls;
- trap and restore focus in modal surfaces;
- announce async status changes where they affect the task;
- honour `prefers-reduced-motion`;
- pair geolocation with an explicit consent action and a manual alternative;
- never encode availability, payment or verification solely in colour.

## Attribution

The experience footer should include:

> A Digital Experience by [SolarSpin Technologies](https://solarspin-namibia.pages.dev/)

Third-party map, type and channel marks remain subject to their own licences and brand rules. Their inclusion in documentation does not imply partnership or approval.
