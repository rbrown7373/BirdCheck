# Source Map — Documentation Provenance

**Audited source:** user-provided October 29, 2026 Xcode archives, overlaid with the October 29 WeatherKit-removal package for planned BirdCheck 1.0 build 8. The user reported a successful Xcode build and resubmission; this documentation pass did not run Xcode or independently inspect an installed release.

| Topic | Source files / evidence |
|---|---|
| Core personal models | `BirdCheck/Bird.swift` |
| Local reference taxonomy | `BirdCheck/BirdDatabase.swift`, `BirdCheck/BirdRegion.swift`, bundled AviList/region resources |
| Startup and CloudKit store split | `BirdCheck/BirdCheckApp.swift` |
| Home and Settings | `BirdCheck/BirdCheckHomeAndSettings.swift` |
| Lists, Life List, daily checklists, Outing details | `BirdCheck/BirdCheckListsAndChecklist.swift` |
| Outings/Sightings archive, Calendar, manual Outing, folders | `BirdCheck/BirdCheckOutingsAndDrawers.swift` |
| Bird detail, photos, added birds, search, regional views | `BirdCheck/BirdCheckRegionsSearchDetail.swift` |
| Map, saved locations | `BirdCheck/BirdCheckMaps.swift` |
| BirdCheck AI presentation/input | `BirdCheck/BirdCheckAIView.swift` |
| AI planning and counting | `BirdCheck/BirdCheckAIQuestionPlanner.swift`, `BirdCheck/BirdCheckAIQueryEngine.swift`, `BirdCheck/BirdCheckAIObservationLedger.swift`, `BirdCheck/BirdCheckAIRecordProjection.swift` and related files |
| Backup format and restore logic | `BirdCheck/BirdCheckBackup.swift`, `BirdCheck/BirdCheckCoreSupport.swift` |
| iPhone↔Watch communication | `BirdCheck/BirdCheckPhoneConnectivity.swift`, Watch app `ContentView.swift`, `BirdCheckWatchConnectivity.swift` |
| Watch Outings and workout recording | `BirdCheck/BirdCheckWatchOutingService.swift`, Watch app `BirdCheckWatchFitnessWorkout.swift` |
| WeatherKit removal baseline | October 29 WeatherKit-removal archive (8 Swift files and `BirdCheck.entitlements`) |

## User-observed validation from development

Selected voice queries, the Colleyville/known-place species reconciliation, six-photo addition, and last-Outing metrics were reported working on a physical iPhone in prior testing. They are **targeted user observations**, not a guarantee every data path, restore workflow, or Watch sync scenario was tested.

## Documentation safety checks

- Do not copy Xcode project files, signing settings, provisioning artifacts, private data stores, or user backups into a public documentation repository.
- Keep implementation notes separate from customer-facing instructions.
- Confirm build/version before updating platform-specific features.
- Cite the original data providers when describing AviList and regional reference data.
