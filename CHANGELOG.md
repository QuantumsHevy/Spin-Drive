# Changelog
All notable user-facing changes to SpinDrive are documented in this file. This mod is compatible with Kerbal Space Program 1.12.5 unless noted otherwise. Version numbers should follow semantic versioning.

## v1.1.0
### Fixed
- Fixed `AstrophageGenerator`'s model rotation to look more like a fuel cell when placed on a craft.
- Fixed all parts' bulkhead profiles to match actual part size (0.3125m, 2.5m, srf).
- Fixed some fuel switches not working due to part-related edge cases. Astrophage fuel switches now piggyback any values from the existing fuel types that previously determined compatibility.
### Added
- Added `VABOrganizer` support. All spin drives are now listed under Spin Drives within Engines, and the Astrophage Fuel Cell is now properly recognized as a fuel cell.
- Added `CommunityCategoryKit` support with a custom "Spin Drives" category filter.
- Added an astrophage KSPIE fuel switch patch: Tanks that use Interstellar Extended's `moduleID = KSPIE` rather than B9's own `moduleID = fuelswitch` now receive the astrophage fuel type as they would without KSPIE.
### Changed
- Improved `AstrophageGenerator`'s title and description (now named "Pepper" Astrophage Fuel Cell).
- Changed the `EnrichedAstrophage` fuel subtype's colors to match what's seen in the *Project Hail Mary* movie.
- Changed the CryoTanks fuel switch patch to look for the `[LH2]` subtype instead of a combined `[LH2/O]` subtype.

## v1.0.3
This is SpinDrive's first official GitHub release. Versions 1.0.0-1.0.2 (below) were previously distributed on SpaceDock only; they're recorded here so the mod has one continuous history, going forward.
### Fixed
- Removed a duplicate, packaged `FarFutureTechnologies.dll` that may conflict with any existing FFT installs.
### Added
- Added an astrophage CryoTanks fuel switch patch: `SUBTYPE[LH2/O]` now can target CryoTanks-native tanks without false-positives on FFT/BlueShift/any other non-`[LF/Ox]` tanks.
- Added `primaryColor` and `secondaryColor` hex fields as well as an `EnrAst` resource bar abbreviation so astrophage now shows up as a red/maroon resource and is abbreviated properly in resource menus.

## v1.0.2
### Fixed
- Fixed a plume naming/compatibility issue so the spin drive cluster uses the intended Waterfall plume again, included a patch to avoid breaking existing craft.

## v1.0.1
### Changed
- Rebalanced the cost of the spin drives and their fuel for career mode.

## v1.0.0
- Initial release.