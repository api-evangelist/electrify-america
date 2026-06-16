# Electrify America (electrify-america)

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
