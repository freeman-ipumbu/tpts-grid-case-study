# Desert Signal · TPTS Countryfront design system

Desert Signal is the public design system for TPTS Grid: a map-native product with the confidence of financial infrastructure and the sensory character of Namibia. The **TPTS Countryfront** is its current cinematic expression—a visual journey that changes atmosphere with Namibia's geography and a complete Desert Day / Astro Night cycle while preserving one calm interaction system.

Each section has one deliberate role: the opening creates desire, Country Pulse adds useful national context, the Navigator creates orientation, the landscape chapters create memory, the factual directory creates trust and onboarding collects evidence.

This is a rationale and token reference, not a distributable copy of the production interface or logo artwork. Product references reflect the production release verified on 18 October 2026.

## Brand idea

**Movement converges into possibility.**

The mark is imagined as route lines meeting at signal nodes: road, place, payment and people becoming one coherent grid. It avoids literal animals, flags and predictable dune silhouettes. The result should feel Namibian through material, light, scale and rhythm—not decoration.

The countryfront extends that idea through the full page. Route threads, topographic lines, horizon gradients and photographic stages connect the experience without behaving like a progress tracker or competing with the map. They are editorial devices; they do not indicate route completion, live position or distance.

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

The system has one semantic palette expressed through two complete light cycles.

| Family | Representative values | Role |
| --- | --- | --- |
| Mineral ink | `#061716`, `#082421`, `#102625` | Astro Night ground, focused geographic surfaces and strong text |
| Desert cream | `#FFF9EC`, `#FBF6EA`, `#F6E6CA` | Desert Day page, paper and sand surfaces |
| Atlantic | `#147C80`, `#2F9C94`, `#73CDC1` | Navigation, focus, active connection and water context |
| Clay | `#923F29`, `#C5643F`, `#E0956E` | Route character, editorial warmth and primary light-theme emphasis |
| Sun | `#DDA64E`, `#F2B84D` | Sparse attention and daylight context |
| Mist | `#DCEBE2`, `#C7D7CE`, `#526460` | Quiet panels, dividers and secondary copy |

**Desert Day** applies cream, sand, mist, Atlantic teal, clay and sun across the entire page. **Astro Night** moves the same hierarchy into mineral green-black, warm ochre, muted clay and luminous aqua. Cards, fields, media overlays, footer, safety surfaces and section transitions all participate; a theme switch is not a header-only recolour.

Colour is semantic, never the only carrier of state. Text and icons keep connected, partial, unavailable, gated and error states legible without hue. Image overlays use theme-specific contrast treatment so the foreground and photography feel related rather than pasted together.

## Typography

- **Brand and display:** [Geologica](https://github.com/googlefonts/geologica) — variable, compact and geological without becoming themed.
- **Interface:** [IBM Plex Sans](https://github.com/IBM/plex) — highly legible controls and longer UI copy.
- **Data:** IBM Plex Mono — coordinates, status labels, route metadata and compact system information.

Geologica carries both structure and emotional scale through deliberate weight, optical-size, shape and spacing choices. IBM Plex Sans keeps ordinary controls and reading relaxed. IBM Plex Mono is a functional layer, not an aesthetic applied to paragraphs. No decorative serif is used in the current release.

## Shape and layout

- compact radii (typically 4–12 px) keep the interface infrastructural;
- strong vertical sections make scroll position legible;
- editorial asymmetry creates surprise without disturbing task flows;
- thin lines and small data labels add precision;
- the cinematic hero uses location-accurate Namibia imagery and a route signal, not a second live map;
- the route workspace reads as one wide instrument—map first, evidence second—rather than two equal dashboard cards;
- each major product chapter has its own geographic atmosphere instead of repeating one solid brand fill;
- progressive postcard and editorial landscape sequences use scale and asymmetry to communicate different environments without flooding the first viewport with equal cards;
- map, imagery and copy overlap only when contrast and pointer behaviour remain unambiguous;
- controls meet a 44 px minimum target, with 48 px preferred for primary actions.

## Motion

Motion should feel like a vehicle settling onto a road: quick, weighted and purposeful.

- entrance motion uses restrained vertical reveal;
- selections have a short spring response;
- the convergence mark can draw its routes and then resolve its nodes;
- countryfront route nodes and atmosphere layers breathe slowly while the page is active, without communicating product state;
- hover lift and image scale run only on devices that actually support hover;
- scroll navigation announces spatial movement without hijacking scroll;
- loading language may sequence “mapping / connecting / opening Namibia” while work is real;
- every non-essential animation has a reduced-motion equivalent.

Do not use endless parallax, decorative cursor trails, forced scroll sequences or animation that delays access to content.

## One-map language

The base map is context; the TPTS overlay is meaning.

- the **Grid Navigator** is the sole always-available traveller map and preserves geographic context across **Discover**, **Build** and **Stays**;
- its visual frame uses measured corner marks, a dark geographic field and a wider map-to-panel ratio so the country—not a control column—holds the scene;
- Discover prioritises destination context, Build prioritises the traveller's ordered line and Stays prioritises factual property points and their synchronized records;
- the live Route OS lives *inside Build* and reuses that map for **Route Truth**, **Daylight Corridor**, **Weather Along Route**, **Route Essentials** and **Living Namibia**; the lenses are views of one route, not five map instances;
- the five-lens dock uses a compact icon, short label, full accessible name and one expanded evidence panel; the selected lens changes overlay emphasis while route order and camera context remain stable;
- Climate Memory and other source-backed summaries sit in a companion signal deck instead of becoming extra maps or pretending that every dataset has precise drawable geometry;
- **Field**, **Atlas** and **Signal** are visual appearances over the same attributed map and product data; a style switch never changes a place's state;
- destination anchors, unclaimed property points and a future bookable state remain visually and textually distinct;
- a planned route uses a strong continuous signal; it is labelled as direct-line journey order until a successful provider response supplies road-following geometry, and even then remains planning guidance rather than navigation;
- lens colour remains secondary to plain-language state: connected, partial, unavailable, credential required, no match and gated are always readable without colour;
- source, evidence date or period, provider state and limitation stay next to material intelligence rather than disappearing into a global legal page;
- attribution remains visible;
- selected markers provide a corresponding text label and detail surface;
- zoom controls are keyboard operable;
- loading, degraded and unavailable states are written in plain language;
- a directory/list view remains usable without the map.

Map restraint is part of the identity. The property directory uses an **Atlas Lens**—regional evidence, record counts and coverage gaps—instead of mounting another map. Owner onboarding mounts a separate precision map only after an explicit request and only to place or review one public-facing point. The two tools are scoped, labelled and never presented as alternate traveller maps.

The current directory has 28 factual property records and 27 sourced OpenStreetMap-derived map points: 17 OSM nodes and 10 explicitly labelled geometry centroids. Their marker treatment communicates “discoverable / unclaimed,” never availability. The remaining record keeps a null coordinate instead of showing a guessed pin.

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
- the Route OS lens dock never blocks ordinary route editing and collapses cleanly on small screens;
- Daylight Corridor exposes the dated shared solar window, Weather exposes time-stamped stop context, and Living Namibia describes bounded EONET awareness plus aggregate count-only GBIF context without suggesting comprehensive hazards or wildlife prediction;
- Route Essentials shows a deliberate empty state until a versioned, attributed Namibia extract is approved—empty visual space is preferable to fabricated or stale pins;
- Climate Memory explicitly says “climatology · not a forecast” and retains its month, sampling boundary and source;
- the live Offline Route Pack action describes a static last-known export, includes generation time and limitations, and never uses the language of live offline navigation;
- inventory, price and road-condition authority never appear in the planning surface.

The five intelligence lenses and the three Navigator task lenses have different hierarchy. Discover / Build / Stays answer “what am I doing?”; Route / Light / Sky / Stops / Living answer “which evidence am I inspecting inside my route?” This distinction keeps the information architecture legible and prevents another row of equal-looking global navigation.

## Country Pulse interaction language

Country Pulse is a place-led planning surface, not another map or a generic weather widget.

- four clearly named Namibia locations switch the image, forecast and contextual summary;
- every location owns a dedicated, unobstructed photograph stage with its caption and source separated from the forecast copy;
- weather, guidance and help form a compact three-card row on wide screens, recompose at tablet widths and reduce to a three-column metric grid on phones;
- temperature, condition, wind, precipitation, sunrise, sunset and climate memory remain grouped by meaning rather than scattered across decorative cards;
- generated travel cues explain the underlying weather signal and never claim to be personalised safety advice;
- the FCDO card shows its source, public update time, scope limitation and Open Government Licence attribution;
- the “Help in Namibia” action opens a focused, keyboard-contained drawer with tap-to-call and copy actions;
- core contact numbers are saved into the traveller-generated Offline Route Pack and a separate static offline safety shell;
- unavailable provider data becomes a named fallback state—never a plausible-looking fake live reading.

## Imagery

Imagery reveals Namibia's scale, texture and transitions: city, Atlantic fog, salt, road, dune, canyon, pan, wildlife, community landscape, river light, architecture, rock art, weather and night sky.

The current homepage uses **33 unique real-photograph families with zero cross-section repetition**:

- four real-photo opening scenes: Deadvlei, Sandwich Harbour, Etosha elephants and the Namibian night sky;
- four dedicated Country Pulse / “Read the Sky” scenes: Windhoek, Swakopmund, Sesriem and Okaukuejo;
- 12 destination postcards;
- an eight-scene Country Atlas spanning the Quiver Tree Forest, Brandberg, Twyfelfontein, Epupa Falls, Popa Falls, Kolmanskop, the Zambezi and Welwitschia country;
- four field-note scenes and one separate Spitzkoppe closing panorama.

The expansion introduced **28 genuinely distinct Wikimedia Commons photographs**. Twenty-seven are assigned once on the homepage, Hardap Dam is retained for a later route or destination surface, and six separately licensed retained photographs complete the 33-slot live sequence. This allocation replaces the previous pattern in which responsive derivatives created the appearance of variety while the same underlying photographs recurred across sections.

Responsive WebP derivatives keep bandwidth and crop control inside the product. Licensed treatment permits resizing, responsive cropping and restrained colour adjustment within the source licence. Visible page-level credits provide immediate source cues, while the footer and [image provenance register](image-provenance.md) preserve the complete record.

All imagery is **destination atmosphere only**. It never stands in for a property image, listing relationship, room, rate, review, availability or booking state. The factual directory continues to omit third-party property photography until a verified operator supplies content it is authorised to use.

The production slot registry and source-level tests treat responsive sizes as derivatives of one visual family—not extra images. They reject duplicate homepage family assignments, incomplete creator/source/licence metadata and missing local WebP candidates. Archived campaign compositions stay outside factual property surfaces and are not part of the current homepage sequence.

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

Current implementation evidence includes a skip link, labelled map regions, keyboard marker buttons, `aria-live` status messages, focus containment/restoration for the command and safety dialogs, theme-aware browser chrome and reduced-motion handling for map movement and decorative reveals. These measures are a maintained baseline, not a claim of formal accessibility certification.

## Responsive and mobile contract

The phone layout is designed as a first-class task surface rather than a scaled desktop canvas:

- the Navigator map and active lens panel stack, and long route lists stop using nested scroll regions;
- postcard and editorial landscape collections become a deliberate vertical sequence with readable credits and focal points instead of shrinking into an illegible desktop mosaic;
- Country Pulse preserves the photograph as a bounded foreground stage instead of placing it behind copy, and the weather panel contracts without swallowing the phone viewport;
- the hero photograph, copy and route composer preserve a clear reading order and useful controls at 320 px, 390 px and wider phone layouts;
- property and integration grids become single-column;
- the mobile dock keeps Explore, Trip, Places and Host within reach, respects safe-area insets and yields while the host precision map is open;
- primary tap targets expand to at least 44 px, with several navigation actions at 46–52 px;
- form controls use 16 px text on phones and keep the onboarding steps readable;
- non-selected marker labels simplify on narrow screens while selected context remains visible;
- property fact panels, provenance and claim/correction actions reflow without removing truth labels;
- long dialogs use viewport-aware maximum heights and scrolling.

The breakpoint work is implementation evidence, not a substitute for ongoing device, keyboard, screen-reader, contrast and zoom testing.

## Install and offline contract

Installability is useful only when its limits remain obvious:

- a browser install affordance appears only when the platform exposes the prompt;
- iOS receives explicit Share → Add to Home Screen guidance;
- the installed experience uses standalone display and theme-aware browser chrome;
- the service worker stores only a bounded public shell and immutable public assets;
- API, owner, listing, booking, checkout and payment responses are never cached for offline replay;
- an offline navigation failure opens a purpose-built safety screen, not a stale imitation of the live marketplace;
- live maps, weather, availability, listings, payments and bookings remain explicitly unavailable offline.

## Attribution

The experience footer should include:

> A Digital Experience by [SolarSpin Technologies](https://www.solarspin-namibia.xyz/)

Third-party map, type and channel marks remain subject to their own licences and brand rules. Their inclusion in documentation does not imply partnership or approval.

Photography attribution, campaign-composition disclosure and adaptation notes are maintained in the [Namibia image provenance register](image-provenance.md). An image source does not imply that its creator or hosting platform endorses TPTS Grid.
