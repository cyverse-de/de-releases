# CyVerse Discovery Environment (DE) Changelog

All notable changes to this project will be documented in this file. The format is based on [Keep a Changelog][1].

## [Unreleased]

### Added

- It is now possible for users to download public data from the Data Store in the Discovery Environment without having
  to log in.
- Discovery Environment administrators can now edit the list of rates associated with a subscription add-on.

### Changed

- A bug that prevented proper redirection for users with pre-existing single sign-on sessions was fixed.

## [v2025.02.04]

### Added

- A list of recent logins will now be displayed on the DE dashboard.
- The Terrain API now supports scheduled changes in rates and quota defaults for both subscriptions and add-ons.
- It is now possible to instruct the DE to associate shared memory volumes with VICE apps by adding a a container device
  to the tool with a `Host Path` of `/dev/shm` and a `Container Path` set to the amount of memory to allocate, for
  example, `8Gi`.

### Changed

- The minimum and maximum CPU usage request fields in the app launch wizard have been replaced by a single CPU request
  field.
- Users who already have a single sign-on session for CyVerse should now be logged in automatically wihtout having to
  click the login button.
- Clicking on binary file types will no longer open the file edit dialog. Instead, the file will simply be downloaded.

## [v2024.12.04]

### Added

- The DE now has the ability to generate HTML source for a badge that can be used to instantly launch an analysis with
  predefined parameters.
- When an analysis launch link is used for an instant launch, the DE will now launch the analysis immediately rather
  than display the analysis launch wizard.
- While analyses are running, perodic notifications will be sent to users in order to remind them that the analysis is
  running. This notification should help to prevent the unintentional consumption of compute hours.
- When an app has multiple versions, anyone with permission to modify the app can change the order of the app versions
  in order to ensure that the most commonly used app versions stay close to the top of the list.

### Changed

- Dependency updates for most microservices.
- The options to terminate and extend the time limit of a job on the analysis summary page are now buttons if there is
  sufficient room on the display.
- The option to request help for an analysis has been moved into the ellipsis menu on the analysis summary page.
- When launching an analysis, the default setting for maximum CPUs requested will be set to 4 CPUs rather than being set
  to the highest number of CPUs that can be requested for the app.
- Fixed a bug that was intermittently preventing the user's current subscription from being retrieved correctly.

### Removed

## [v3.1.2]

This is the initial release using this deployment method.

[Unreleased]: https://github.com/cyverse-de/de-releases/compare/v2025.02.04...HEAD
[v2025.02.04]: https://github.com/cyverse-de/de-releases/compare/v2024.12.04...v2025.02.04
[v2024.12.04]: https://github.com/cyverse-de/de-releases/compare/v3.1.2...v2024.12.04
[v3.1.2]: https://github.com/cyverse-de/de-releases/compare/v0.0.7...v3.1.2
[1]: https://keepachangelog.com/en/1.1.0/
