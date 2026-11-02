# Backups, Restore and iCloud

Your personal records deserve careful handling. BirdCheck uses a **CloudKit-backed personal database** for supported user data, separate from its local bundled bird and region reference catalog. It also has local automatic and manual backup snapshots.

## Automatic Backup

In **Settings → Backup & Restore**, BirdCheck shows the time of the latest **Automatic Backup**. The app checks whether personal data has changed when opening/returning to BirdCheck, after a short delay, and refreshes its automatic backup when needed. It is **not** a guarantee that a backup is written immediately after every tap.

## Manual Backup

Select **Settings → Back Up Now** to capture a current manual backup. The source describes two retained local backup slots: an **Automatic Backup** and a **Manual Backup**. Creating another manual backup replaces the previous manual backup slot; it does not merge two archives.

## What is in the backup?

The personal-data snapshot contains lists, list folders, checked birds and counts, bird photos **including their image bytes and primary-photo selection**, user-added birds, custom regions, known locations, and Outing/Sighting session data. Bird names and region reference databases are bundled with the app and are reconstructed instead of copied into each personal backup.

## Restoring

**Settings → Restore…** lets you choose an available automatic or manual backup and inspect details before confirming. Restoration is a significant data operation; it is **not a general-purpose merge of two independently edited libraries**. Read all warnings and previews and avoid starting a restore merely to refresh iCloud synchronization.

## iCloud syncing

BirdCheck's personal SwiftData store is configured with a **private CloudKit database**. Changes may synchronize asynchronously and can take time to appear on another device using the relevant iCloud account and app setup. A count shown locally does not, by itself, prove the data reached the cloud or another device.

## If something looks missing

1. Do not delete BirdCheck or erase its data.
2. Check whether you're signed in to the expected iCloud account.
3. Reopen BirdCheck on the device with the existing records and allow synchronization time.
4. Check **Settings → Backup & Restore** dates before making any restore decision.
5. Contact support with the device, build, steps, and a non-sensitive description. **Never send a complete personal backup to public GitHub issues.**

## Legacy migration safeguards

The project contains a migration path that preserves a pre-cloud personal-data safety snapshot and refuses to silently substitute a blank personal store if a database cannot open. These protections do not replace testing a restore or maintaining a separate personal backup when available.
