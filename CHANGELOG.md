## 3.3.4 - 2018-09-05
### Fixed
- Fixed a bug where SimpleMap would not validate required fields. (via @samhibberd)

## 3.3.3 - 2018-03-13
### Fixed
- Fixed a bug where SimpleMap would cause the `ResaveElements` job to error when triggered via console.

## 3.3.2 - 2018-03-05
### Added
- Added docs for using a config file to configure the plugin.

### Fixed
- Fixed JOIN alias issue when using the Element API plugin (via @idontmessabout)

## 3.3.1 - 2018-01-30
### Fixed
- Fixed JS bug on settings page

## 3.3.0 - 2018-01-30
### Fixed
- Added a fix for those annoying `Call to a member function getMap() on null` bugs

### Improved
- Map height no longer jumps when page loads
- Vastly improved the map fields settings UI/UX
	- No more nasty text fields!
	- Map height and position is now set by resizing and moving a map
	- Auto-complete search bounds can now be drawn directly onto a map
	- Radio buttons are now drop-downs

### Changed
- Now using the plugins `afterInstall` function instead of the plugin after install event
- The "Hide Lat/Lng" option is now true by default

## 3.2.0 - 2018-01-25
### Fixed
- Fixed bug where pagination would error when querying via a map field. #70

### Improved
- Updated CraftQL support (via @markhuot)
- Removed webonyx/graphql-php dependency #71
- Improved address and lat/lng input sizing on smaller screens and in a HUD #73
- Updated Mapbox example to use latest API #74

## 3.1.3 - 2017-12-18
### Fixed
- Map fields no longer cause global sets to fail to save!

## 3.1.2 - 2017-12-18
### Fixed
- Fixed settings not translating for non-English languages
- Fixed boundary settings fields not accepting decimals

## 3.1.1 - 2017-11-30
### Fixed
- Fixed bug where maps were failing to save.

## 3.1.0 - 2017-11-30
### Added
- [CraftQL](https://github.com/markhuot/craftql) support!
- Added `craft.simpleMap.getLatLngFromAddress($addressString[, $country])`.

### Improved
- The maps `parts` now contains all available options from [here](https://developers.google.com/maps/documentation/geocoding/intro#Types) (including the `_small` variants). Any options without values are returned as empty strings.

## 3.0.4 - 2017-11-28
### Added
- Added ability to restrict location search by country

### Changed
- New icon!

## 3.0.3 - 2017-11-08
### Added
- It's now possible to save the map field with only an address! Useful for populating the field from the front-end. (Requires the Geocoding API).

### Improved
- The address and lat/lng are now validated.

## 3.0.2 - 2017-11-03
### Fixed
- Fixed a bug where location searches would error if `orderBy` was not defined

## 3.0.1 - 2017-11-03
### Fixed
- Fixed maps not rendering

## 3.0.0 - 2017-11-03
### Changed
- Initial Craft 3 Release
