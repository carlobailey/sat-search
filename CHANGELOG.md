# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## Changed
- Updated to work with [STAC API v0.9.0-rc1](https://github.com/radiantearth/stac-spec/blob/master/CHANGELOG.md#v090-rc1---2020-01-06)
- `SATUTILS_API_URL` envvar changed to `STAC_API_URL`

## [v0.2.2] - 2019-09-20

### Changed
- Parser module now handles reading JSON from file
- sat-stac dependency bumped to 0.3.0 - tests updated
- requestor-pays CLI switch, and requestor_pays keyword arg now properly spelled as requester-pays and requester_pays

### Fixed
- Fixed issue with some comparison ops not being evaluated

## [v0.2.1] - 2019-02-14

### Fixed
- Fix number found reported when using .found() function and searching by IDs
- Fixed URL paths in windows by using urljoin instead of os.path.join

### Changed
- update default API URL to sat-api.developmentseed.org
- update default save path from ${eo:platform}/${date} to ${collection}/${date}
- Default limit to search.items() changed from 1000 to 10000
- Changed internal page size from 1000 to 500 (page size of queries to endpoint)

### Added
- Warning issued when number of items found greater than limit
- requestor-pays option to acknowledge paying of egress costs when downloading (defaults to False)


## [v0.2.0] - 2019-01-31

### Changed
- Works with version 0.2.0 of sat-api (STAC 0.6.x)
- Major refactor, uses sat-stac library


## [v0.1.0] - 2018-10-25

Initial Release

[Unreleased]: https://github.com/sat-utils/sat-search/compare/master...develop
[v0.2.2]: https://github.com/sat-utils/sat-search/compare/0.2.1...v0.2.2
[v0.2.1]: https://github.com/sat-utils/sat-search/compare/0.2.0...v0.2.1
[v0.2.0]: https://github.com/sat-utils/sat-search/compare/0.1.0...v0.2.0
[v0.1.0]: https://github.com/sat-utils/sat-search/tree/0.1.0
