# Documentation Verification and Maintenance

This handbook is a **source-grounded first draft** for BirdCheck 1.0 build 8, created while the corrected app version was awaiting Apple review. It is not itself proof of an approved release or a complete production-device audit.

## Verified in source

- Home navigation labels and the Outing/Sighting entry points
- Settings preference labels and available backup choices
- Personal data models, Life List provenance, bird photo records and geographic fields
- Six-photo gallery and starred-primary selection
- Local automatic/manual backup snapshot and CloudKit-backed personal store configuration
- WeatherKit removal package and preservation of manual/historical weather fields
- Apple Watch interface labels and Fitness/birding-only choices

## User-reported device checks from development

- Voice-based personal-region, date, last-Outing and comparison questions in specific examples
- AI and Map both reporting the same 26 distinct species for one test city/place
- Adding photos to a bird card
- Xcode building after the WeatherKit correction

## Not independently verified in this documentation pass

- End-to-end restoration from an actual six-photo backup on a new device
- Current production CloudKit propagation across multiple devices
- Every Apple Watch communication failure mode
- Exact final screenshots and wording in the App Store-approved binary
- Whether Apple has approved the pending app review

## Before publishing on GitHub

1. Confirm the latest approved app **version/build**.
2. Compare every navigational instruction against that binary and update anything that differs.
3. Confirm screenshots are from that same build and contain no personal details.
4. Review privacy and data-handling statements with the official Privacy Policy.
5. Confirm taxonomy/version and third-party attribution.
6. Test every link and revise the AI reference when behavior changes.
7. Keep draft or uncertain features clearly labeled; never silently turn them into supported claims.

## Updating later

Every app release should update the `README.md` version note, this verification page, relevant workflows, and `llms.txt`. Whenever a bug fix changes semantics—such as personal counting, location identity, or backup behavior—update the corresponding FAQ and AI reference as well. The documentation should match **shipped behavior**, not just intended architecture.
