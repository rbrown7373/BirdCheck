# Settings, Permissions and Privacy

Open **Settings** from BirdCheck Home.

## Main settings

- **How BirdCheck Works:** Replay the built-in introduction.
- **iPhone Automatic Location:** Control automatic GPS capture on this iPhone. Manual place search remains available.
- **iPhone Voice Recording:** Control iPhone speech input, subject to microphone/speech-recognition permissions.
- **Automatically Add to Life List:** Determine whether birds checked on other lists are added to the Life List; switching it off does not remove already checked birds.
- **Show Live Outing Map:** Set the default live-map visibility. Hiding the map does not itself stop location recording.
- **Record Outings to Apple Fitness:** Request Health access for iPhone-started Outings; Watch-started Outings use a separate Watch choice.
- **Backup & Restore:** See automatic/manual backup times, back up now, inspect a restore choice.
- **Bird Data:** AviList taxonomy and regional data credits.
- **Privacy & Support:** Links to the published Privacy Policy and Support & FAQ.
- **Erase All Personal Data:** A destructive action that must not be used as a normal sync troubleshooting step.

## Permission troubleshooting

Some capabilities rely on Apple's system permissions in addition to BirdCheck preferences:

- **Location:** Routes and place information may be unavailable when permission is denied.
- **Microphone / Speech Recognition:** Needed for iPhone voice questions and supported Watch voice actions.
- **Apple Health / Fitness:** Only needed for relevant health/fitness recording; bird checklists can function without it.
- **Photos / Camera:** Used when selecting or taking your own bird pictures.

If a permission is missing, check both BirdCheck's preference and the relevant Apple system permission. An app-specific toggle cannot override a denied iOS authorization.

## Weather data in build 8

BirdCheck 1.0 build 8 **does not support live WeatherKit retrieval**. It retains fields for existing or manually entered weather-related information on Outings and Sightings. Do not claim that the app currently obtains Apple Weather forecasts.

## Information-sharing boundaries

Personal data is distinct from the locally bundled reference bird catalog. iCloud synchronization uses the user's private CloudKit context when available; do not infer that any individual user's sync has completed solely from this design. See the actual linked privacy policy for legally authoritative data-handling terms.

Public support requests should avoid precise coordinates, detailed personal schedules, sensitive health information, backup files, and account identifiers.
