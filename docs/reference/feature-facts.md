# BirdCheck 1.0 — Authoritative Feature Facts

**Product:** BirdCheck (iPhone companion app with Apple Watch functionality). **Source baseline:** October 29, 2026 project archives with the WeatherKit removal update for 1.0 build 8. **Status:** documentation draft, not a certification of App Review approval.

## User-visible capabilities supported by source

| Feature | What the source supports | What not to imply |
|---|---|---|
| Life List | Checked species with manual/observation provenance | Not a dated personal observation for every entry |
| Reusable Lists | Lists, checkmarks, counts, folders, optional regional/location context | Not the same as a catalog distribution map |
| Outings | Dated birding sessions, bird checklist, optional route/activity/notes | Fitness metrics are not always available |
| Quick Sightings | Non-walking way to record one or more birds | Does not require a walking route |
| Map | Personal observations and saved geographic evidence | Does not invent geolocations from a place name |
| Bird Cards | Species details, observation history, saved known places | Not a built-in image library for every species |
| My Photos | Up to six user photos, one starred primary, full-screen zoom/pan | Not six photos in addition to the main image |
| BirdCheck AI | Questions over saved personal evidence and reference catalog, voice input | External assistants cannot see the user's database |
| Apple Watch | Outings, spoken bird addition, Fitness/birding-only choices | Not independent proof that all records synced to iPhone |
| CloudKit | Cloud-backed private personal store | No guarantee that sync is instantaneous |
| Backups | Local automatic and manual snapshots with personal data and image bytes | Do not describe as a merge/sync replacement |
| Weather | Retains historical/manual conditions fields | **No live WeatherKit in build 8** |

## Reference data and attribution

The project Settings screen identifies **AviList v2025b**, licensed under **CC BY 4.0**, as the worldwide taxonomy and describes regional occurrence data derived from the **eBird Observation Dataset via GBIF**. Reference-range information is separate from the user's confirmed sightings.

## Reliability principles

1. Data is the source of truth; AI, Map, and other interfaces should query the same personal evidence.
2. Count **distinct species** separately from **recorded individual birds**.
3. Life List evidence can establish a species as seen even if it has no dated Outing.
4. A regional Life List entry requires regional evidence; a globally checked species does not automatically belong to every state.
5. Never fabricate observation dates, individual counts, geographic locations, photographs, or iCloud success.
6. If the app needs clarification, explain precisely which ambiguity remains.
