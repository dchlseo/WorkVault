# Data and analysis catalog
Reviewed 2026-11-09 KST. Definitions below are read from existing analysis documentation; no raw-data recalculation was performed.

| Dataset / analysis | Definition and period as reported | Evidence and use |
|---|---|---|
| KAC international departing passengers | 2025 monthly departures, airport/partner airport/carrier/nationality/sex/age; Incheon excluded | [L0031 review](Evidence/L0031.md), [provider dialogue L0077](Evidence/L0077.md); route/carrier structure |
| Ministry of Justice immigration | Monthly airport-level entries/exits and Korean/foreign totals | KAC review QA comparison; does not provide the same route/carrier detail |
| Airportal international operations | 2016.01–2026.10; 2020–2022 not included; monthly airport × counterpart × carrier | [L0162](Evidence/L0162.md), [L0244](Evidence/L0244.md); exploratory supply/network/carrier analysis |
| Korea visitor survey | 2025 survey rental-car proxy from expense/prebooking; source README reports n=16,110 | [L0118](Evidence/L0118.md); no movement legs, per-leg mode or entry/exit airport |
| Japan FF-Data | Movement/transport evidence used in comparative rental-car deck | [L0439](../LastMile/Evidence/L0439.md); reconcile persons/legs and weights before cross-country comparison |
| Airport international schedules | Preparation source describes 2026/27 winter planned flights | [November 6 preparation](../Strategy/Evidence/Drive-20261106-preparation.md); planned schedules are not actual slot headroom |
| Telecom OD | Definitions and handover still to be clarified in preparation source | Device/person/movement, expansion weights, suppression, nationality, airport identification and stay definitions need verification |
| IATA sample | Preparation source reports sample requested; available product/variables unconfirmed | Do not infer data received, licence scope or city/carrier-level estimates |

## Reproducibility pointers
Local KAC data directory contains analysis notebooks, generated tables and report builders. Airportal README describes QA, network trends, carrier structure, entry/exit episodes, candidate markets and event studies.
Use original source code/data and record versions before regenerating results. This task did not execute source analysis, alter data or verify reported statistics.

## Material limitations
KAC departures are not person-level inbound arrivals. Full-year airport totals may be compared with immigration statistics within documented limits; do not extend that approximation to individual routes/carriers.
Airportal EDA uses departures+arrivals and distinguishes ordinary international passenger operations. Its “ten-year” title does not mean uninterrupted annual coverage.
Keep forecast, potential demand, past traffic, available seats, flight plans and operating capacity distinct.

Raw files and outputs are linked by ID in the [data source register](README.md). Local paths and Drive candidate matches are in [reconciliation](../Sources/Reconciliation.md).

