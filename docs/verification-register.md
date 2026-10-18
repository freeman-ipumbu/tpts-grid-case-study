# Public verification register

This register records the evidence used for time-sensitive statements in the case study. It contains no credentials, application records, private correspondence, host contact details or provider-issued implementation material.

Last reviewed: **18 October 2026**

## Product-owned release evidence

| Subject | Evidence checked | Public statement supported |
| --- | --- | --- |
| Grid Navigator | Current product source and release walkthrough | One shared traveller map with Discover, Build and Stays task lenses; lens changes preserve one geographic workspace while changing the active overlay and controls. |
| Build lens | Current product source and release walkthrough; [earlier Route Studio capture](../assets/tpts-grid-route-studio-live-2026-10-16.jpg) retained as release history | Empty-start route editor with search, add, remove, reorder, trip name/nights, local save, deliberate share and non-navigation disclaimers. The linked image predates the unified Navigator information architecture. |
| TPTS Road Intelligence | Current production endpoint, desktop walkthrough, responsive walkthrough and routed production smoke test | Live MET Norway forecasts at selected destination anchors; production-connected openrouteservice geometry and estimates are accepted only through the bounded server adapter; direct-line fallback visibly withholds road kilometres and drive time. |
| Route OS | Production deployment from reviewed private runtime revision `c8000f6`; desktop, phone, maximum-route and routed-provider walkthroughs on 18 October 2026 | One Build map exposes Route Truth, Daylight Corridor, Weather Along Route, Route Essentials and Living Namibia as five switchable lenses without creating competing maps. |
| Daylight Corridor | Production schema-v2 routed maximum-route response | MET Norway Sunrise 3.0 returned dated solar context for 12/12 selected stops and a shared window; daylight remained independently available alongside routed road truth. |
| Climate Memory | Production schema-v2 maximum-route response | NASA POWER returned monthly climatology for 4/12 evenly sampled stops and remained labelled as regional historical context, not current weather. |
| Natural-event and biodiversity context | Two production maximum-route responses plus deep schema validation | EONET returned a valid connected empty state; GBIF returned connected aggregate count-only context. No GBIF occurrence records, taxa names, coordinates or media were exposed. |
| Route Essentials | Production map and empty-state walkthrough | The fifth lens is live, but no unverified objects are drawn while the governed, versioned Namibia extract remains gated. |
| Offline Route Pack | Production export-path walkthrough | The generated static file contains the chosen route, latest available context, sources, generation time and limitations. It is not an offline basemap, navigation service or self-updating alert channel. |
| Map appearances | Current production map configuration | Field, Atlas and Signal select three OpenFreeMap styles without changing product state or data. |
| Cinematic opening | Current product source and responsive walkthrough | Location-accurate Namibia imagery, route-signal motion and search/composer actions hand off into the relevant Navigator lens; no competing hero map is mounted. |
| Public property index | Current factual directory module evaluated on 16 October 2026 | 28 records; 27 non-null exact OSM points; every record is unclaimed, has no inventory and is not represented as a TPTS partner. |
| Atlas Lens | Current property-directory surface | Regional record distribution and coverage gaps replace the prior directory map; selected sets open in the Navigator's Stays lens. |
| Claim and correction | Current directory cards and factual record pages | Every record has a claim path and an account-free correction/removal path. Claiming still requires authority verification. |
| Owner onboarding | Current three-step form, validation contract and intake state machine | Public point and operating facts can enter a private `verification_required` queue; its precision map opens only on explicit request and submission does not publish or create inventory. |
| Owner authentication and account access | Current customer-surface review and identity boundary | Gated pending TPTS-owned identity; no authenticated owner workspace is claimed live on the canonical Cloudflare customer surface. |
| Integration launchpad | Deployed 29-record readiness catalogue and production provider checks | One owned path, seven live paths, two ready paths, six apply paths, ten evaluate paths and three restricted paths; no ready/apply/evaluate record is represented as a credential, approval or live-inventory claim. |
| Payment boundary | Production readiness surface and server-side configuration check | Payment mode is disabled; partner diagnostics are configured and read-only; distinct merchant credentials are absent; live payment creation and automatic paid-state confirmation are disabled. |
| Dependency audit | Current lockfile, pnpm 11.25.0, `pnpm audit --prod --json` and `pnpm audit --json` | Production scope reported 0 advisories. Full graph reported 34 development-path advisories: 15 high, 13 moderate, 6 low and 0 critical. |

The retained screenshot is evidence of the earlier rendered Route Studio surface only. It predates the unified Grid Navigator and does not prove current information architecture, inventory, OTA access, merchant activation, payment success or accessibility conformance.

## Production verification observations

The following observations were captured against [tpts-grid.pages.dev](https://tpts-grid.pages.dev) on 18 October 2026. The openrouteservice activation checks used the activation deployment's deployment-specific hostname; the provider secret remained environment configuration.

| Check | Observed result | Interpretation limit |
| --- | --- | --- |
| Public surfaces | Root, owner, integrations and payment-readiness surfaces each returned HTTP 200 | Availability of a shell does not activate owner authentication, inventory, payment creation or a marketplace |
| Map worker | Same-origin MapLibre worker returned HTTP 200 as `application/javascript`, 508,314 bytes | Transfer success does not prove every tile source or future device will remain available |
| Browser QA | Production walkthrough at 696 px produced no console errors or horizontal overflow; separate 390 px and 320 px responsive layout checks produced no horizontal overflow | Release checks, not formal accessibility certification or exhaustive device coverage |
| Initial openrouteservice activation request | Degraded to direct-line truth and withheld road metrics; the response was not written to the normalized TPTS edge cache after the failed attempted ORS route | A failed provider response cannot masquerade as road routing or poison the normalized TPTS edge cache; no broader claim about public cache headers is made |
| Stable one-leg openrouteservice request | On hardened runtime `c8000f6`, HTTP 200 with cache `MISS` in 1,418 ms; `truthState: routed`; `providerState: connected`; 2,029 geometry points; 628.1 km; 362 minutes; one routed leg | Point-in-time provider evidence, not turn-by-turn navigation, live access, safety authority, an SLA or a universal estimate |
| Exact one-leg routed repeat | Cache `HIT` in 54 ms with the same routed truth | Confirms the tested exact-repeat cache path, not a universal response-time commitment |
| Routed maximum-route fresh request | A fresh 12-stop route returned HTTP 200 with cache `MISS` in 4,955 ms; routing was routed/connected with 9,719 geometry points, 2,778.5 km, 2,173 minutes and 11 routed legs | One point-in-time maximum-route observation, not an SLA, safety verdict or universal estimate |
| Routed maximum-route provider sections | Schema v2 valid; weather 12/12; daylight 12/12; climate 4/12 sampled; EONET connected explicit-empty with zero matches; GBIF connected count-only at 434,697 | Provider completeness and road safety are not implied; explicit-empty EONET means only no matching open result, and the GBIF aggregate predicts no sighting |
| Exact maximum-route repeat | Cache `HIT` in 67 ms with the same routed truth; no authorization value or JWT-shaped secret was exposed | Confirms the tested exact-repeat cache path, not a universal response-time commitment |
| Runtime tail | Cloudflare reported `outcome: ok` with 32 ms CPU time for an earlier observed request | Isolate CPU measurement is not end-to-end network latency or a capacity promise |
| Payment boundary | Mode disabled; partner diagnostics configured; distinct merchant credentials absent | No checkout, charge, merchant processing or automatic paid-state confirmation is live |

The 12-stop checks exercise the maximum accepted route size. The separate one-leg openrouteservice checks verify the degraded-to-connected activation sequence and exact-repeat cache path. Neither set of checks turns public context into emergency, access, navigation, traffic, closure or wildlife authority.

## External programme and data sources

| Subject | Official source | Public fact used in this case study |
| --- | --- | --- |
| Booking.com Demand API | [Prerequisites](https://developers.booking.com/demand/docs/getting-started/prerequisites) | Managed Affiliate Partner registration, Partner Centre access and issued credentials are prerequisites; secrets must not be published. |
| Booking.com Connectivity | [Connectivity portal](https://connect.booking.com/?lang=en) | New connectivity-provider integrations are paused until further notice; direct individual-property connections are not accepted. |
| Expedia Rapid | [Getting started](https://developers.expediagroup.com/rapid/setup) | Partner status, restricted development, site review and production enablement are distinct gates. |
| Expedia lodging connectivity | [Connectivity Hub](https://developers.expediagroup.com/supply/lodging) | The public path includes contact, PCI/licence review, consultation, development/testing and go-live; direct individual-property connections are not accepted. |
| Hostelworld | [Affiliate programme](https://partners.hostelworld.com/) | Applications are reviewed; links, creative assets, feeds and deeper solutions are programme options, not automatic API access. |
| Hotelbeds / HBX | [Getting started](https://developer.hotelbeds.com/documentation/getting-started/) | Registration provides evaluation access; testing does not create real reservations or charges and later environments remain gated. |
| ResRequest ResConnect | [Connection process](https://support.resrequest.com/resconnect/develop-a-connection-to-resconnect/) | Development requires an NDA and sandbox request, followed by an audit before go-live. |
| NightsBridge | [Channel management](https://site.nightsbridge.com/features/channel-management/) | NightsBridge publicly presents regional channel-management capability; the page is a commercial pathway, not a public developer-access grant to TPTS. |
| Google Hotel Center | [Hotel Prices integration overview](https://developers.google.com/hotels/hotel-prices/dev-guide/data-feeds) | Free booking links require eligible properties plus maintained hotel, rate, availability and landing-page data; directory facts alone are insufficient. |
| Travelgate Hotel-X | [API overview](https://docs.travelgate.com/docs/apis/overview/) | Travelgate publishes an aggregation API surface; supplier rights and a commercial relationship still govern usable inventory. |
| Channex | [Start integration](https://channex.io/start-integration) | A staging environment exists, but production requires testing, certification and OTA account authorisation. |
| Wetu | [Connect API](https://knowledge.wetu.com/connect-apiincoming) | The incoming Connect API requires registration and a test key and is aimed at itinerary/booking presentation workflows. |
| Amadeus Hotels | [Enterprise hotel APIs](https://developers.amadeus.com/enterprise/category/hotel) | Hotel access is treated as an enterprise evaluation path; TPTS does not claim credentials or approval. |
| Airbnb | [Software partners](https://www.airbnb.com/software-partners) | Software access is a governed partner pathway, not a public directory seed or permission to scrape. |
| CallPay merchant integration | [General merchant terms](https://www.callpay.com/merchant-general-terms/) | Merchant acceptance and service-specific Integration Documents precede service activation; public terms are not a complete payment specification. |
| OpenStreetMap data | [Copyright and licence](https://www.openstreetmap.org/copyright) and [OSMF legal FAQ](https://osmfoundation.org/wiki/Licence_and_Legal_FAQ) | Map facts require attribution and ODbL-aware handling; an OSM point does not imply a commercial relationship. |
| OpenFreeMap | [openfreemap.org](https://openfreemap.org/) | Public style service used by Field, Atlas and Signal map modes. |
| MET Norway Locationforecast | [Terms of service](https://api.met.no/doc/TermsOfService) and [Locationforecast guide](https://api.met.no/doc/locationforecast/HowTO) | Public global point forecasts require an identifying user agent, responsible caching and attribution; forecasts are context, not safety advice. |
| MET Norway Sunrise 3.0 | [API documentation](https://api.met.no/weatherapi/sunrise/3.0/documentation) | The public service provides dated solar and lunar events for coordinates; calculated daylight does not establish visibility, road condition or personal safety. |
| openrouteservice | [Developer portal](https://openrouteservice.org/dev/) and [service restrictions](https://openrouteservice.org/restrictions/) | The TPTS bounded server adapter is production-connected and returned road geometry, distance and estimated duration in a public smoke test. Its tested direct-line fallback withholds road metrics when routing is unavailable; no key or provider response turns the product into navigation, access or safety authority. |
| NASA POWER | [API documentation](https://power.larc.nasa.gov/docs/services/api/) | Historical and climatological parameters are useful for regional season context when period and spatial resolution remain visible; they are not a local current forecast. |
| GBIF | [API reference](https://techdocs.gbif.org/en/openapi/) | The live public layer exposes only an aggregate five-year count for a bounded route envelope. Occurrence records may be incomplete, historical or spatially sensitive, so records, taxa, coordinates and media are not returned to the browser and no sighting is predicted. |
| OSM Route Essentials | [Overpass API](https://wiki.openstreetmap.org/wiki/Overpass_API) and [OSM copyright](https://www.openstreetmap.org/copyright) | Mapped service points require attribution and incomplete-data warnings; TPTS intends versioned hosted extracts rather than a public Overpass instance in each traveller request. |
| Wikidata and Wikimedia Commons | [API usage guidelines](https://foundation.wikimedia.org/wiki/Policy:Wikimedia_Foundation_API_Usage_Guidelines) | Destination facts and media require revision-aware provenance plus per-item author and licence handling. |
| NASA EONET | [API v3 documentation](https://eonet.gsfc.nasa.gov/docs/v3) | Open natural-event metadata can provide dated regional awareness; it is not an official emergency, closure, evacuation or navigation service. |
| Frankfurter | [frankfurter.dev](https://frankfurter.dev/) | No-key reference exchange-rate data is available; any future display conversion must remain indicative and separate from a canonical NAD price. |
| Cloudflare Turnstile | [Product documentation](https://developers.cloudflare.com/turnstile/) | A free challenge path exists, but server-side Siteverify and issued widget credentials are required before activation. |
| NASA FIRMS | [Area API](https://firms.modaps.eosdis.nasa.gov/api/area/) | Active-fire observations are an evaluation path for separately labelled awareness context, not a current routing or safety feature. |
| MapLibre offline regions | [Native offline guide](https://maplibre.org/maplibre-native-ffi/guides/work-offline/) | Managed offline regions are a native capability, not proof that the browser export stores licensed map tiles; native versus bounded PWA architecture and deletion rules remain evaluation work. |
| TPTS privacy and contact | [Privacy policy](https://www.tptsnam.com/privacy-policy/) and [contact](https://www.tptsnam.com/contact/) | Operative privacy information and the public channel for product, property and correction enquiries. |

## Interpretation rules

- **Discoverable** means a factual public shell; it does not mean claimed, verified, partnered or bookable.
- **Claimed** means authority has been verified; it does not mean rates or inventory are live.
- **Bookable** requires separately activated inventory, policies, commercial authority and a working payment/reconciliation path.
- **Owner authentication gated** means the public claim and submission paths exist without live owner account access; an authenticated workspace requires a future TPTS-owned identity boundary.
- **Path verified** means an official application or documentation path exists; it does **not** mean TPTS has been approved.
- **Live** means deployed provider-backed behaviour and its fallback were production-verified; it does not mean complete coverage, commercial partnership or safety authority.
- **Ready** means a documented technical path exists but activation or governance evidence is incomplete; it is not production access.
- **Activation gated** means an architectural boundary exists but production use still depends on legal, commercial, security, provider and operational requirements.
- **Production verified** records a dated release observation. It is not an uptime, latency, accessibility or provider-coverage guarantee.
- **Freshness available** means the relevant observation, forecast, evidence period, lookback or generation time is exposed; it does not make the source complete or authoritative for safety.
- **No matching result** means only that the bounded query returned none. It must not be translated into “no event,” “no species” or “no essential service exists.”
- Dependency audits are registry snapshots, not security guarantees. Re-run both production-only and full-graph audits after every lockfile change.
- Provider pages and programme terms can change. Re-check this register before making a new public status claim.
