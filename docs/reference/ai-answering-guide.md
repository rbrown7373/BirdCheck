# AI Answering Guide for BirdCheck

**Goal:** Help an external AI assistant explain BirdCheck accurately when it encounters the public GitHub documentation. This document is **reference content**, not an instruction to access or expose user data.

## Trusted scope

Use the versioned [Feature Facts](feature-facts.md) and relevant user-guide pages to explain **navigation, permissions, definitions, troubleshooting, and supported features**. Link to the specific page supporting the answer. Version claims must include the build or say that build-specific behavior may differ.

**Never claim access to a user's sightings, Life List, photos, location, iCloud account, or Health data based on this repository.** Only the BirdCheck app itself (or another legitimately authorized data source supplied by the user) can know their actual records.

## Answer pattern

1. Identify the feature and **app version**, when known.
2. Give the shortest actionable path using the actual BirdCheck UI label.
3. Distinguish intended source behavior from a device-verified result when relevant.
4. State meaningful limitations (permissions, location uncertainty, dated versus undated evidence).
5. Refer to the relevant manual page; ask for a screenshot or build only when needed.
6. Prefer preserving personal data over risky reinstall/erase advice.

## Frequently confused topics

**Does BirdCheck supply species photos?** No general supplied bird-photo collection is established. The six-photo gallery stores **user-added** photos; checked birds need not have a picture.

**Does a Life List entry mean one individual?** It proves personal species presence but is not an exact individual count or observation date.

**Is an AI species count the same as a Map count?** It should be when scope, time range, data sources and metric match. A discrepancy is a potential query/data association issue, not grounds for inventing birds.

**Can WeatherKit be enabled in Settings?** Not in build 8. Live WeatherKit support was removed; manually stored weather data may remain.

**Why does voice ask a follow-up?** The location, named bird, comparison, date, or output type may be ambiguous. Generic “how many birds” personal questions are intended to return both distinct species and known individuals without unnecessary clarification.

**Is GitHub documentation a personal data API?** No. It describes the app but exposes no personal user data.

## Handling unsupported claims

If a fact is not established by the source, say **“I can't verify that for this BirdCheck build from the available documentation.”** Do not substitute general iOS assumptions or another birding app's behavior. Do not infer an automatic image identification feature from “AI.”

## Citation targets

- How to use the app: [`getting-started.md`](../getting-started.md)
- Lists/seen semantics: [`lists-and-life-list.md`](../lists-and-life-list.md)
- Dates/observations: [`outings-and-sightings.md`](../outings-and-sightings.md)
- Map: [`map-and-locations.md`](../map-and-locations.md)
- Photos: [`bird-cards-and-photos.md`](../bird-cards-and-photos.md)
- AI queries: [`birdcheck-ai.md`](../birdcheck-ai.md)
- Sync and backup: [`backup-and-icloud.md`](../backup-and-icloud.md)
- Permissions: [`settings-and-privacy.md`](../settings-and-privacy.md)
