# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
## [1.4.0] 2012-02-07
- Memory consumption is fixed

## [1.3.1] 2012-02-07
- added operation name and arguments in to the error details

## [1.3.0] 2018-05-16
- added opts to Blunder.Absinthe.add_error_handling

## [1.2.1] 2018-05-04
- fixed compilation warning

## [1.2.0] 2018-05-03
## Added
- configurable Bugsnag reporting depending on severity

## [1.1.2] 2018-05-01
- original error is reported to bugsnag instead of blunder error
- added a stacktrace to a bugsnag report

## [1.1.1] 2018-04-23
### Fixed
- More context and metadata sent to bugsnag in Bugsnag error handler.

## [1.1.0] 2018-04-19
Added error handling for `Absinthe.Middleware.Async`

## [1.0.1] 2018-04-02
First public release

## [1.0.0] 2018-02-18
### Changed
- Exception handling no longer added around the default `MapGet` resolver middleware. This gives a dramatic performance improvement.
### Added
- `Blunder.Absinthe.Dataloader.SafeKV` added to provide exception handling in KV Dataloaders
### Fixed
- Absinthe middleware can be specified in the middleware list by a bare module name (atom). We were not handling this case in `add_error_handling`
- Just adding blunder-absinthe to your mixfile caused runtime errors since there was no default error handler list. Making `LogError` the default.

## [0.1.2] 2018-02-13
### Fixed
- Added credo and coveralls and fixed the issues they surfaced

## [0.1.1] 2018-02-13
Fix compiler warnings

## [0.1.0] 2018-02-13
Initial extraction of logic from Blunder
