# Desert Signal design system

Desert Signal is the public design direction for TPTS Grid: a map-native digital product with the confidence of financial infrastructure and the sensory character of Namibia. Each section has one deliberate role: the opening creates desire, the Navigator creates orientation, the Atlas Lens creates trust and onboarding collects evidence.

This is a rationale and token reference, not a distributable copy of the production interface or logo artwork. Product references reflect the 18 October 2026 discovery-pilot release.

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
- the cinematic hero uses location-accurate Namibia imagery and a route signal, not a second live map;
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

## One-map language

The base map is context; the TPTS overlay is meaning.

- the **Grid Navigator** is the sole always-available traveller map and preserves geographic context across **Discover**, **Build** and **Stays**;
- Discover prioritises destination context, Build prioritises the traveller's ordered line and Stays prioritises factual property points and their synchronized records;
- **Field**, **Atlas** and **Signal** are visual appearances over the same attributed map and product data; a style switch never changes a place's state;
- destination anchors, unclaimed property points and a future bookable state remain visually and textually distinct;
- a planned route uses a strong continuous signal; it is labelled as direct-line journey order until a successful provider response supplies road-following geometry, and even then remains planning guidance rather than navigation;
- attribution remains visible;
- selected markers provide a corresponding text label and detail surface;
- zoom controls are keyboard operable;
- loading, degraded and unavailable states are written in plain language;
- a directory/list view remains usable without the map.

Map restraint is part of the identity. The property directory uses an **Atlas Lens**—regional evidence, record counts and coverage gaps—instead of mounting another map. Owner onboarding mounts a separate precision map only after an explicit request and only to place or review one public-facing point. The two tools are scoped, labelled and never presented as alternate traveller maps.

The current directory has 28 factual property records and 27 exact OSM points. Their marker treatment communicates “discoverable / unclaimed,” never availability. The remaining record keeps a null coordinate instead of showing a guessed pin.

## Grid Navigator interaction language

The Navigator changes controls through task lenses without moving the traveller into a different product:

- Discover searches destinations and offers explicit routes into planning or nearby factual stays;
- Build begins empty and makes ownership of the plan visible;
- Stays keeps map selection and the factual result list synchronized;
- story-led prompts and directory actions open the relevant lens directly.

Within Build:

- searching and adding are separate, explicit actions;
- every stop has named move-earlier, move-later and remove controls;
- trip name and nights are ordinary editable fields;
- the optional Grid Guide explains a suggestion and offers a reversible action;
- local saving and sharing are described separately;
- direct-line kilometres carry an asterisk and plain-language warning;
- road kilometres and drive time appear only for a successful routing-provider response, while live point weather names its public source;
- inventory, price and road-condition authority never appear in the planning surface.

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

Current implementation evidence includes a skip link, labelled map regions, keyboard marker buttons, `aria-live` status messages, focus containment/restoration for the command dialog and reduced-motion handling for map movement and decorative reveals. These measures are a maintained baseline, not a claim of formal accessibility certification.

## Responsive and mobile contract

The phone layout is designed as a first-class task surface rather than a scaled desktop canvas:

- the Navigator map and active lens panel stack, and long route lists stop using nested scroll regions;
- property and integration grids become single-column;
- the mobile dock keeps Explore, Trip, Places and Host within reach, respects safe-area insets and yields while the host precision map is open;
- primary tap targets expand to at least 44 px, with several navigation actions at 46–52 px;
- form controls use 16 px text on phones and keep the onboarding steps readable;
- non-selected marker labels simplify on narrow screens while selected context remains visible;
- property fact panels, provenance and claim/correction actions reflow without removing truth labels;
- long dialogs use viewport-aware maximum heights and scrolling.

The breakpoint work is implementation evidence, not a substitute for ongoing device, keyboard, screen-reader, contrast and zoom testing.

## Attribution

The experience footer should include:

> A Digital Experience by [SolarSpin Technologies](https://solarspin-namibia.pages.dev/)

Third-party map, type and channel marks remain subject to their own licences and brand rules. Their inclusion in documentation does not imply partnership or approval.
