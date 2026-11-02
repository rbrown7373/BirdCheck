# Outings and Sightings

## Which should I use?

**Outing:** A birding session, often a walk, with a start time, end time, species entries, and potentially route and fitness information. Start it with the green **Let's Go Birding** control on Home. When active, use **Return to Birding** to resume.

**Sighting:** A faster way to record one or more birds without starting a full walking session. Start it with the blue **New Sighting** control. A Sighting can save when and where birds were recorded, even when no walking route exists.

Internally, BirdCheck's current quick-Sighting flow uses an `Outing`-style record marked as a Sighting. That is an implementation detail; users should use whichever Home action fits what they are doing.

## Recording an Outing

1. Tap **Let's Go Birding** on the Home screen (or start an Outing on Apple Watch).
2. Add each bird species as you encounter it; record the number of individual birds when known.
3. Optionally use the live map. **Hiding the map does not stop route or observation-location capture** when the relevant location permissions and settings allow recording.
4. Use the Outing controls to end it; the app saves a completed record and displays a summary.
5. Find completed records under **Outings & Sightings**, **Recent**, **Calendar**, or the dated archive.

An Outing can include a bird checklist, location information, notes, route samples, and other activity statistics. Some fitness metrics depend on permissions and device availability.

## Recording a quick Sighting

1. Tap **New Sighting**.
2. Add the bird or birds you saw and their counts.
3. Review the time and location. A manual place entry can be used if GPS is unavailable or undesired.
4. Finish and save the record.

Quick Sightings contribute personal birding evidence and should appear in relevant history and geographical questions, even if no Outing route was created.

## Historical entries and editing

The **Outings & Sightings** archive provides a manual **Add Outing** path. Existing records expose an **Edit Outing** or **Edit Sighting** screen for available date, time, location, conditions, and notes fields. A manually entered historical record should reflect what you actually know; omit or leave uncertain details unset where possible.

BirdCheck preserves geographic levels such as **country → state → city → place** when those are available. A local place name, a friendly name, and GPS coordinates are not identical things. See [Map and locations](map-and-locations.md).

## Deleting records and the Life List

Deleting an Outing or Sighting can affect the evidence supporting automatically added Life List species. BirdCheck may offer options such as **Delete & Keep Life List** and **Delete & Remove from Life List**. Manually added or separately supported Life List records are protected by provenance rules. Read the actual confirmation before proceeding.

## Weather in version 1.0 build 8

**Automatic WeatherKit retrieval was removed** in build 8 because it was not working. Older saved weather values and manually editable conditions fields are preserved. Do not expect BirdCheck to fetch live Apple Weather conditions in this build.

## Common questions

- Can I record a Sighting without a walking Outing? **Yes.**
- Does hiding the live map disable GPS collection? **No, not by itself.**
- Is one checked species the same as one individual bird? **No.**
- Can a record exist without precise GPS? **Yes, location can be optional or manually entered.**
