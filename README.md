# Electrify America (electrify-america)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Electrify America is the largest open EV fast-charging network in the United States, operating more than 5,600 DC fast chargers at over 1,080 locations across the US and Canada. Subsidiary of Volkswagen Group of America, the network offers charging speeds up to 350 kW and supports CCS, CHAdeMO, and NACS connectors. Electrify America provides REST APIs through a partner developer portal that enables automotive OEMs and enterprise integrators to locate charging stations, check real-time charger availability, retrieve session pricing, and manage charging sessions. Authentication is handled via OAuth2 / Auth0. A consumer-facing mobile app (iOS/Android) provides pass-based subscription plans (Pass and Pass+) with per-kWh pricing, and the Plug&Charge standard (ISO 15118) is supported at all stations for certificate-based auto-authentication.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/electrify-america/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/electrify-america/refs/heads/main/apis.yml)

## Tags

- Electric Vehicles
- EV Charging
- Charging Stations
- DC Fast Charging
- Plug and Charge
- Automotive
- Energy
- Transportation
- Mobility

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### Electrify America Stations API

REST API for locating and querying Electrify America charging stations. Enables partners and OEM integrators to search for stations by geographic area or coordinates, retrieve station details (address, connectors, amenities), and filter by connector type (CCS, CHAdeMO, NACS) or charging speed. Access requires OAuth2 partner credentials issued through the Electrify America developer portal.

- **Human URL:** [https://developer.electrifyamerica.com/](https://developer.electrifyamerica.com/)
- **Base URL:** `https://api.electrifyamerica.com`

#### Tags

- Charging Stations
- Location
- Station Search
- Connectors

#### Properties

- [Documentation](https://developer.electrifyamerica.com/)
- [Authentication](https://developer.electrifyamerica.com/)

### Electrify America Availability API

Real-time charger availability API that returns live connector status (available, in-use, faulted, offline) for individual charging stations and EVSE units. Used by automotive OEM in-vehicle navigation and mobile app partners to surface live availability before and during a journey. Requires OAuth2 partner credentials.

- **Human URL:** [https://developer.electrifyamerica.com/](https://developer.electrifyamerica.com/)
- **Base URL:** `https://api.electrifyamerica.com`

#### Tags

- Real-Time
- Availability
- Charger Status
- EVSE

#### Properties

- [Documentation](https://developer.electrifyamerica.com/)
- [Press Release](https://media.electrifyamerica.com/releases/273)

### Electrify America Pricing API

API providing per-session and per-kWh pricing data for Electrify America charging stations. Supports time-of-use (TOU) pricing retrieval so partners and in-vehicle systems can display accurate session cost estimates before a driver plugs in. Pricing varies by location, charger, and time of day.

- **Human URL:** [https://developer.electrifyamerica.com/](https://developer.electrifyamerica.com/)
- **Base URL:** `https://api.electrifyamerica.com`

#### Tags

- Pricing
- Time-of-Use
- Session Cost
- kWh Rates

#### Properties

- [Documentation](https://developer.electrifyamerica.com/)
- [Pricing](https://www.electrifyamerica.com/pricing/)

### Electrify America Sessions API

API for initiating, monitoring, and retrieving data for EV charging sessions. Enables partner applications to start and stop charging sessions, poll live session telemetry (energy delivered, duration, cost), and retrieve historical session records. Plug&Charge (ISO 15118) is supported at all stations and leverages the Hubject Intercharge PKI for certificate-based authentication as an alternative to session API token flows.

- **Human URL:** [https://developer.electrifyamerica.com/](https://developer.electrifyamerica.com/)
- **Base URL:** `https://api.electrifyamerica.com`

#### Tags

- Charging Sessions
- Plug and Charge
- ISO 15118
- Session Management
- Telemetry

#### Properties

- [Documentation](https://developer.electrifyamerica.com/)
- [Authentication](https://developer.electrifyamerica.com/)

## Common Properties

- [Website](https://www.electrifyamerica.com)
- [Portal](https://developer.electrifyamerica.com)
- [Sign Up](https://developer.electrifyamerica.com)
- [Mobile App](https://apps.apple.com/us/app/electrify-america/id1458030456)
- [Mobile App](https://play.google.com/store/apps/details?id=com.ea.evowner)
- [Pricing](https://www.electrifyamerica.com/pricing/)
- [Status Page](https://cloud.email.electrifyamerica.com/network-and-planned-maintenance)
- [Newsroom](https://media.electrifyamerica.com/)
- [F A Q](https://www.electrifyamerica.com/mobile-faq/)
- [Station Locator](https://www.electrifyamerica.com/locate-charger/)
- [LinkedIn](https://www.linkedin.com/company/electrify-america)
- [Twitter](https://x.com/ElectrifyAm)
- [Plans](plans/plans.yml)
- [Rate Limits](rate-limits/rate-limits.yml)
- [Fin Ops](finops/finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
