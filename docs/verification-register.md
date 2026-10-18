# Public verification register

**Reviewed:** 18 October 2026

**Canonical production surface:** [tpts-grid.pages.dev](https://tpts-grid.pages.dev)

This register records dated public evidence and the limits attached to it. It contains no credentials, private source, internal endpoint inventory, customer information, raw payment-provider material or confidential agreement.

## Current release evidence

| Product claim | Evidence reviewed | What the evidence supports |
| --- | --- | --- |
| Production release | Reviewed private revision `28fb7aeef581cb90851b71b0d3e1abc03f477e7a`; type check, lint, 13/13 automated tests and production build | The current release passed its dated engineering gate; this is not an uptime or defect-free guarantee |
| Delivery | Canonical root, manifest, service worker and offline safety page returned HTTP 200; response included security headers | The public shell and install/offline assets were available at the test time |
| Responsive behaviour | Wide desktop, laptop, tablet and 390/320 px phone walkthroughs in Desert Day and Astro Night | No horizontal overflow or console errors were observed across the hero, Country Pulse, compact weather module, Country Atlas and closing manifesto in the tested flows; this is not formal accessibility certification |
| Countryfront | Current production UI and theme rules | Desert Day and Astro Night affect full sections, cards, fields, imagery overlays and browser theme colour—not only the navigation bar |
| Typography | Production font imports and rendered hierarchy | Geologica is the brand/display family; IBM Plex Sans is the interface family; IBM Plex Mono is the data/status family; Newsreader is not part of the current system |
| Image system | Canonical 33-slot visual registry, production footer register and [public image register](image-provenance.md) | 33 unique real-photo homepage families with zero cross-section reuse; 28 were newly sourced from Wikimedia Commons and none is property or inventory evidence |
| Image source tests | Four source-level visual tests | Exactly 33 unique semantic assignments, complete creator/source/licence records and existing local responsive WebP candidates; these tests do not replace human crop or licence review |
| Destination layer | Current public destination module | 27 geographic anchors for route context; an anchor is not inventory or a safety/access claim |
| Grid Navigator | Current production interaction and responsive walkthrough | One persistent traveller map exposes Discover, Build and Stays primary lenses; subordinate Build evidence views reuse the same map |
| Route ownership | Build interaction walkthrough | Travellers can begin empty, add/remove/reorder up to 12 stops, edit trip name and duration, save locally, share deliberately and export a static pack |
| Public property index | Current factual directory module | 28 records: 17 OSM nodes, 10 labelled OSM geometry centroids and 1 record with no guessed point; every record remains unclaimed and non-bookable |
| Claim and correction | Public record and onboarding flows | Every stay exposes claim and account-free correction/removal routes; a claim still requires authority verification |
| Owner onboarding | Three-step form and intake state | Submission creates a private verification-required draft; it does not publish, create inventory or make a stay bookable |
| Country Pulse | Production weather/context surface and responsive walkthrough | Each location has dedicated unobstructed imagery; latest-model weather/daylight, regional climate memory, FCDO source links and verified contacts appear in a compact responsive composition with source and scope limitations |
| Help in Namibia | Production safety drawer and offline screen | Sourced contacts include 112, 10111, 9682, Windhoek response, Tourist Protection and the Ministry helpline; TPTS does not triage or guarantee connection |
| PWA installability | Standalone manifest, browser install handling, iOS guidance, icons and service worker | The site is installable where supported; offline support is limited to a public safety shell and safe static assets |
| Offline data boundary | Service-worker rules and offline page | API, owner, listing, booking, checkout and payment responses are excluded from cache; stale content is not presented as current live data |
| Integration catalogue | Current 35-record public catalogue | 1 owned, 8 live, 3 build-ready, 8 apply, 12 evaluate and 3 restricted; non-live stages do not imply access or approval |
| OneGate boundary | Public readiness surface and guarded server contract | Partner scope is read-only; merchant payment creation and automatic paid-state confirmation remain disabled |

The retained [Route Studio screenshot](../assets/tpts-grid-route-studio-live-2026-10-16.jpg) is historical evidence only. It predates the current countryfront and does not prove inventory, OTA access, payment activation or the current responsive information architecture.

## Production API observations

The following point-in-time observations were made against the canonical production surface on 18 October 2026:

| Check | Observed result | Interpretation limit |
| --- | --- | --- |
| Single-anchor road intelligence request | HTTP 200, schema v2; MET weather, MET Sunrise, NASA POWER, EONET and count-only GBIF sections reported connected provider states | A single anchor correctly remains direct-line context with no road leg; connected sources do not imply complete coverage or safety authority |
| Natural-event context | Connected NASA EONET response with no matching event in the bounded request | “No match” does not mean no hazard exists; EONET is not an official emergency or closure feed |
| Biodiversity context | Connected, aggregate-only GBIF mode | No record-level species, coordinate or media payload is claimed; an aggregate never predicts a sighting |
| Travel-advice request | HTTP 200; direct Namibia guidance link, public update time and Open Government Licence v3.0 disclosure | General UK FCDO guidance, not personalised visa clearance, Namibian authority advice or a safety guarantee |
| Routing boundary | openrouteservice is the production routed-road provider; direct-line fallback remains explicit; the provider deadline is eight seconds | A route line or drive estimate is planning context, not navigation, traffic, access, closure or safety authority |
| Route cache policy | Automated policy tests plus a cold and exact-repeat production request | Healthy direct/routed responses use 300-second client and 900-second edge freshness; failed ORS-mode responses use a 120-second isolated fallback cache and continue to withhold road metrics |
| Routed production smoke | Cold request returned routed/connected road truth in 1.43 seconds; exact repeat returned in 0.295 seconds with an edge cache hit | Point-in-time evidence for the tested two-stop route, not an SLA or complete provider-coverage claim |
| Payment readiness | Live creation disabled; partner diagnostic limited to authorised read-only scope | No checkout, charge, merchant processing or automatic payment confirmation is live |

Provider data changes, and public programme terms can change. These observations are dated evidence, not an SLA.

## Integration programme register

The names below link to the official public programme or documentation page used for classification. A link proves that a path was researched; it does not prove credentials, approval, a contract or a TPTS partnership.

| Stage | Path | Public posture |
| --- | --- | --- |
| Owned | [TPTS Direct](https://tpts-grid.pages.dev/#host) | Owned foundation |
| Live | [OpenStreetMap foundation](https://www.openstreetmap.org/copyright) | Live with attribution |
| Live | [MET Norway Weather](https://api.met.no/doc/TermsOfService) | Live forecast context |
| Live | [openrouteservice](https://openrouteservice.org/dev/) | Live routed-road context |
| Live | [MET Norway Sunrise 3.0](https://api.met.no/weatherapi/sunrise/3.0/documentation) | Live daylight context |
| Live | [NASA POWER](https://power.larc.nasa.gov/docs/services/api/) | Live climate memory |
| Live | [GBIF Biodiversity](https://techdocs.gbif.org/en/openapi/) | Live count-only context |
| Live | [NASA EONET](https://eonet.gsfc.nasa.gov/docs/v3) | Live bounded awareness |
| Live | [GOV.UK Content API](https://content-api.publishing.service.gov.uk/reference.html) | Live dated guidance |
| Build-ready | [OSM Route Essentials](https://wiki.openstreetmap.org/wiki/Overpass_API) | Scheduled snapshot path |
| Build-ready | [Wikidata + Wikimedia Commons](https://foundation.wikimedia.org/wiki/Policy:Wikimedia_Foundation_API_Usage_Guidelines) | Open knowledge pathway |
| Build-ready | [GDACS](https://www.gdacs.org/gdacsapi/swagger/index.html) | Open hazard-awareness path |
| Apply | [Nager.Date v4](https://nagerholidays.com/scalar/) | Commercial sponsorship required |
| Apply | [Open-Meteo Air Quality](https://open-meteo.com/en/pricing) | Paid commercial plan required |
| Apply | [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api/overview) | Business setup required |
| Apply | [Booking.com Demand](https://developers.booking.com/demand/docs/getting-started/prerequisites) | Managed Affiliate Partner application required |
| Apply | [Expedia Rapid](https://developers.expediagroup.com/rapid/setup) | Partner review required |
| Apply | [Hostelworld](https://partners.hostelworld.com/) | Affiliate path available |
| Apply | [ResRequest ResConnect](https://support.resrequest.com/resconnect/develop-a-connection-to-resconnect/) | NDA, sandbox and audit path |
| Apply | [NightsBridge](https://site.nightsbridge.com/features/channel-management/) | Commercial relationship required; no public developer API is assumed |
| Evaluate | [GlobalPetrolPrices API](https://www.globalpetrolprices.com/data_access.php) | Quote and data licence |
| Evaluate | [Smithsonian Open Access](https://edan.si.edu/openaccess/apidocs/) | Human-reviewed editorial pilot |
| Evaluate | [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/api/) | MAP key and hazard-language review required |
| Evaluate | [Cloudflare Workers AI + Vectorize](https://developers.cloudflare.com/workers-ai/platform/data-usage/) | Grounding, citation, privacy and retention review |
| Evaluate | [TPTS Offline Grid Pack](https://maplibre.org/maplibre-native-ffi/guides/work-offline/) | Native/PWA and tile-rights gate |
| Evaluate | [Frankfurter FX](https://frankfurter.dev/) | Reference-rate limitation; no direct NAD rate claim |
| Evaluate | [Cloudflare Turnstile](https://developers.cloudflare.com/turnstile/) | Issued keys and server-side verification required |
| Evaluate | [Hotelbeds / HBX](https://developer.hotelbeds.com/documentation/getting-started/) | Evaluation environment, then commercial/certification gates |
| Evaluate | [Google Hotel Center](https://developers.google.com/hotels/hotel-prices/dev-guide/data-feeds) | Inventory and price-feed maturity gate |
| Evaluate | [Travelgate Hotel-X](https://docs.travelgate.com/docs/apis/overview/) | Commercial and supplier-rights evaluation |
| Evaluate | [Channex](https://channex.io/start-integration) | Staging precedes testing/certification |
| Evaluate | [Wetu](https://knowledge.wetu.com/connect-apiincoming) | Registered, licensed content connection |
| Restricted | [Booking.com Connectivity](https://connect.booking.com/?lang=en) | New connectivity-provider intake paused; distinct from Demand |
| Restricted | [Amadeus Hotels](https://developers.amadeus.com/enterprise/category/hotel) | Enterprise-only path |
| Restricted | [Airbnb](https://www.airbnb.com/software-partners) | Approved software partners only; no scraping |

## Payment and trust sources

| Subject | Official source | Public fact used |
| --- | --- | --- |
| CallPay merchant integration | [General merchant terms](https://www.callpay.com/merchant-general-terms/) | Merchant acceptance and service-specific integration documents precede activation; public terms are not a complete payment specification |
| TPTS privacy | [Privacy policy](https://www.tptsnam.com/privacy-policy/) | Operative privacy information for product and owner-submission handling |
| TPTS contact | [Contact](https://www.tptsnam.com/contact/) | Public channel for product, property and correction enquiries |
| Namibia photography | [Public image provenance](image-provenance.md) | Creator/source/licence records for the expanded real-photo atlas plus explicit supply-truth boundaries |

## Interpretation rules

- **Discoverable** means a factual public shell; it does not mean claimed, verified, partnered or bookable.
- **Claimed** means authority has been verified; it does not mean rates or inventory are live.
- **Bookable** requires separately activated inventory, policies, commercial authority and a working payment/reconciliation path.
- **Live** means deployed provider-backed behaviour and an explicit failure path were verified; it does not mean complete coverage, partnership or safety authority.
- **Build-ready** means a documented technical path exists but activation or governance evidence is incomplete; it is not production access.
- **Apply** records a legitimate application or commercial path; it does not mean TPTS has applied or been approved.
- **No matching result** means only that the bounded query returned none. It cannot be translated into “no hazard,” “no species” or “no essential service exists.”
- **Production verified** records dated observations. It is not an uptime, latency, accessibility or provider-coverage guarantee.
- Provider pages, programme intake and pricing can change. Re-check official sources before making a new public status claim.
