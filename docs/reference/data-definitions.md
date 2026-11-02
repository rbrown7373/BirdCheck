# Data Definitions and Counting Rules

This page is intended for both product support and AI-assisted retrieval. Distinguish concepts before answering.

## Terms

- **Bird / species:** A catalog bird identity with common and scientific names, taxonomy, and a durable identifier (normally an Avibase ID). User-added birds have a separate durable user-owned identity.
- **Life List:** A user's collection of bird species marked seen. Membership may be explicitly retained or supported by another observation/list; it need not have an observation date.
- **Checklist / List:** A reusable or date-associated group of bird entries with checkmarks and possibly per-entry individual counts.
- **Outing:** A birding session that can contain multiple species and dated observations, optional route, location, notes and fitness data.
- **Quick Sighting:** A saved bird-recording session without a full walking Outing. The current quick-Sighting implementation uses a `BirdOuting` record with `isSighting = true`.
- **Observation sample:** A timestamped bird entry, potentially with a count and GPS coordinates.
- **Known Location:** A user-recorded bird location that can establish geographic species presence but does not necessarily carry a dated individual total.
- **Reference region:** Geographic occurrence/catalog information; not a claim that the user saw each catalog species.
- **Individual count:** Sum of known quantities in qualifying observations after deduplication; don't use Life List membership as an exact count.
- **Distinct species count:** Number of unique species identities across qualifying personal evidence.
- **Primary photo:** The one starred photo chosen from the species' gallery of up to six images.

## Personal versus reference questions

| User wording | Type of answer |
|---|---|
| “Which birds occur in Texas?” | Reference/catalog occurrence |
| “Which birds have I seen in Texas?” | Personal history with Texas evidence |
| “How many birds have I seen in Texas?” | Personal distinct species and known recorded individuals |
| “How many birds did I see last week?” | Dated observations in that time window |
| “Which birds in Colorado have I not seen in Texas?” | Directional personal set difference: Colorado minus Texas |

## Correctness rules

- Deduplicate the same species across Outings, quick Sightings, Life List, and known-location evidence.
- Do not double-count a Sighting's checklist and observation samples as independent individuals when they describe the same recorded event.
- Count a globally seen Life List bird in a named state **only when** its personal saved evidence connects it to that state.
- Do not force undated Life List evidence into a question about a specific calendar year.
- Use saved structured geography or verified place association for city/state containment; don't assume that a short name belongs to one city globally.
- Same query scope + same data + same metric should yield the same result in Map and BirdCheck AI.

## Worked hypothetical example

Suppose a user has 23 distinct species and 56 recorded individuals in one Outing, plus three additional species only supported by dated Sightings or a geographically supported Life List. The regional species total is a **union** of qualifying unique species, not the sum of each source's raw totals. Additional Life List-only species do not automatically contribute an exact individual count. These numbers are **fictional examples**, not a person's actual BirdCheck data.
