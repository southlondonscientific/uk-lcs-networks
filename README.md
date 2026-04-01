# UK Low-Cost Air Quality Sensor Networks

An open catalogue of low-cost sensor (LCS) air quality monitoring networks operating across the United Kingdom.

## What this is

This dataset catalogues every low-cost air quality sensor network we've been able to identify in the UK as of April 2026. For each network, we record location, scale, ownership, sensor technology, data availability, status, and — where we can determine it — what the data is actually being used for.

The dataset currently contains **44 networks** spanning council deployments, research programmes, citizen science initiatives, and sector-specific monitoring (ports, rail, airports).

## Why it exists

The UK's LCS landscape has grown rapidly, but there's no single place to see what's deployed where. This makes it harder for councils considering sensor purchases, researchers looking for collaboration, and anyone trying to understand how air quality monitoring is evolving. We built this to fill that gap.

## Browse the data

**[Interactive map](https://southlondonscientific.github.io/uk-lcs-networks/map/)** — Leaflet map showing all networks, filterable by status and usage type.

**[CSV dataset](data/uk-lcs-networks.csv)** — The full dataset with 16 columns including coordinates and source URLs.

**[GeoJSON](data/uk-lcs-networks.geojson)** — For programmatic use or importing into GIS tools.

## Data fields

| Field | Description |
|-------|-------------|
| Network Name | Common name of the network or deployment |
| Geography | Location(s) covered |
| Scale (No. Sensors) | Number of sensors deployed |
| Owner / Operator | Organisation(s) running the network |
| Funder(s) | Funding source(s) |
| Sensor Type / Brand | Hardware used |
| Pollutants Measured | PM2.5, NO2, O3, etc. |
| Data Availability | Open, restricted, dashboard-only, etc. |
| Primary Goals | Stated purpose of the network |
| Status (Apr 2026) | Active, Completed, Planned |
| Start Year | Year the network began operating |
| End Year | Year the network ceased (if applicable) |
| Notes / Key Findings | Notable outcomes or context |
| Source / URL | Primary web reference |
| Latitude | Approximate centroid latitude |
| Longitude | Approximate centroid longitude |

## Contributing

We want this to be a living resource. If you know of a network we've missed, or can correct or update an entry, please contribute.

**To add or update a network:**

1. Fork this repository
2. Edit `data/uk-lcs-networks.csv` (please maintain the column structure)
3. Submit a pull request with a brief description of the change

**What we're looking for:**

- Networks we've missed entirely (there will be some)
- Status updates (active networks that have closed, or new ones that have launched)
- Corrections to sensor counts, dates, or ownership
- Better coordinates for multi-site networks

**Guidelines:**

- One network per row. Multi-city programmes (like RSSB rail stations) get a single row.
- Use approximate centroid coordinates for the primary deployment area.
- Include a source URL wherever possible.

We don't gatekeep contributions, but we do check for accuracy before merging.

## Scope

This catalogue covers networks using low-cost sensors (typically <£5,000 per unit), as distinct from reference-grade monitoring stations in the AURN, SAQN, or local authority continuous monitoring networks. We include both active and completed networks to provide a historical view.

"Low-cost" broadly aligns with the definition in PAS 4023:2024 and the Defra LAQM guidance (FAQ 140/148), though we interpret it pragmatically rather than rigidly.

## Limitations

- **Survivorship bias**: Active networks are easier to find than ones that quietly stopped. The true attrition rate is likely higher than this dataset suggests.
- **Coordinates are approximate**: Most are city/borough centroids, not exact sensor locations.
- **Point-in-time snapshot**: The dataset reflects what we could find as of April 2026. Things change.

## Licence

This dataset is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You're free to use, share, and adapt it with attribution.

## Maintained by

[South London Scientific Ltd](https://southlondonscientific.com) — air quality science, exposure assessment, and analytical tools for cleaner air.

Questions or suggestions? Open an issue or email hello@southlondonscientific.com.
