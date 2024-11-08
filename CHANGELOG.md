# CyVerse Discovery Environment (DE) Changelog

All notable changes to this project will be documented in this file. The format is based on [Keep a Changelog][1].

## [Unreleased]

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

[Unreleased]: https://github.com/cyverse-de/de-releases/compare/v3.1.2...HEAD
[v3.1.2]: https://github.com/cyverse-de/de-releases/compare/v0.0.7...v3.1.2
[1]: https://keepachangelog.com/en/1.1.0/
