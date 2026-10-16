# Public verification register

This register records the evidence used for time-sensitive statements in the case study. It contains no credentials, application records, private correspondence, host contact details or provider-issued implementation material.

Last reviewed: **16 October 2026**

## Product-owned release evidence

| Subject | Evidence checked | Public statement supported |
| --- | --- | --- |
| Route Studio | Current product source and release walkthrough; [representative capture](../assets/tpts-grid-route-studio-live-2026-10-16.jpg) | Empty-start route editor with search, add, remove, reorder, trip name/nights, local save, deliberate share and non-navigation disclaimers. |
| Map modes | Current production map configuration | Field, Atlas and Signal select three OpenFreeMap styles without changing product state or data. |
| Public property index | Current factual directory module evaluated on 16 October 2026 | 28 records; 27 non-null exact OSM points; every record is unclaimed, has no inventory and is not represented as a TPTS partner. |
| Claim and correction | Current directory cards and factual record pages | Every record has a claim path and an account-free correction/removal path. Claiming still requires authority verification. |
| Owner onboarding | Current three-step form, validation contract and intake state machine | Public point and operating facts can enter a private `verification_required` queue; submission does not publish or create inventory. |
| Owner workspace | Current signed-in workspace and server identity boundary | Read-only status for applications tied to the verified account; no owner-side mutation, operator token, publication or inventory activation. Non-Sites identity fails closed. |
| Integration launchpad | Current 15-record public readiness catalogue | One owned path, one attribution-ready public-data path, five apply paths, five evaluate paths and three restricted paths; no live connection claim. |
| Payment boundary | Current readiness UI and server-side payment boundary | Partner diagnostics are read-only; live payment creation and automatic paid-state confirmation are disabled. |
| Dependency audit | Current lockfile, pnpm 11.25.0, `pnpm audit --prod --json` and `pnpm audit --json` | Production scope reported 0 advisories. Full graph reported 34 development-path advisories: 15 high, 13 moderate, 6 low and 0 critical. |

The screenshot is evidence of the rendered Route Studio surface only. It does not prove inventory, OTA access, merchant activation, payment success or accessibility conformance.

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
| Google Hotel Center | [Connectivity partner guide](https://support.google.com/hotelprices/answer/11947461?hl=en) | Free booking links require real property, rate, availability and landing-page data plus onboarding/testing; directory facts alone are insufficient. |
| Travelgate Hotel-X | [API overview](https://docs.travelgate.com/docs/apis/overview/) | Travelgate publishes an aggregation API surface; supplier rights and a commercial relationship still govern usable inventory. |
| Channex | [Start integration](https://channex.io/start-integration) | A staging environment exists, but production requires testing, certification and OTA account authorisation. |
| Wetu | [Connect API](https://knowledge.wetu.com/connect-apiincoming) | The incoming Connect API requires registration and a test key and is aimed at itinerary/booking presentation workflows. |
| Amadeus Hotels | [Enterprise hotel APIs](https://developers.amadeus.com/enterprise/category/hotel) | Hotel access is treated as an enterprise evaluation path; TPTS does not claim credentials or approval. |
| Airbnb | [Software partners](https://www.airbnb.com/software-partners) | Software access is a governed partner pathway, not a public directory seed or permission to scrape. |
| CallPay merchant integration | [General merchant terms](https://www.callpay.com/merchant-general-terms/) | Merchant acceptance and service-specific Integration Documents precede service activation; public terms are not a complete payment specification. |
| OpenStreetMap data | [Copyright and licence](https://www.openstreetmap.org/copyright) and [OSMF legal FAQ](https://osmfoundation.org/wiki/Licence_and_Legal_FAQ) | Map facts require attribution and ODbL-aware handling; an OSM point does not imply a commercial relationship. |
| OpenFreeMap | [openfreemap.org](https://openfreemap.org/) | Public style service used by Field, Atlas and Signal map modes. |
| TPTS privacy and contact | [Privacy policy](https://www.tptsnam.com/privacy-policy/) and [contact](https://www.tptsnam.com/contact/) | Operative privacy information and the public channel for product, property and correction enquiries. |

## Interpretation rules

- **Discoverable** means a factual public shell; it does not mean claimed, verified, partnered or bookable.
- **Claimed** means authority has been verified; it does not mean rates or inventory are live.
- **Bookable** requires separately activated inventory, policies, commercial authority and a working payment/reconciliation path.
- **Path verified** means an official application or documentation path exists; it does **not** mean TPTS has been approved.
- **Ready with attribution** applies only to public factual/geographic data, not rates or availability.
- **Activation gated** means an architectural boundary exists but production use still depends on legal, commercial, security, provider and operational requirements.
- Dependency audits are registry snapshots, not security guarantees. Re-run both production-only and full-graph audits after every lockfile change.
- Provider pages and programme terms can change. Re-check this register before making a new public status claim.
