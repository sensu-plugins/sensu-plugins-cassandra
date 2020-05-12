# Change Log
This project adheres to [Semantic Versioning](http://semver.org/).

This CHANGELOG follows the format listed [here](https://github.com/sensu-plugins/community/blob/master/HOW_WE_CHANGELOG.md)

## [Unreleased]

## [3.0.1] - 2020-05-12
### Changed
- Nothing, rolled version to force Travis build after failure

## [3.0.0] - 2020-05-12
### Breaking Changes
- Update minimum required ruby version to 2.3. Drop unsupported ruby versions.
- Bump `sensu-plugin` dependency to `~> 4.0`

### Added
- Bonsai asset support

### Changed
- Updated english dependency to '0.7.0'
- Updated bundler dependency to '~> 2.1'
- Updated rubocop dependency to '~> 0.81.0'
- Remediated rubocop issues
- Updated rake dependency to '~> 13.0'
- Update codeclimate-test-reporter to '~> 1.0'
- metrics-cassandra-graphite.rb: Added support for Row Cache in Cassandra 3.0+

## [2.1.0] - 2019-03-04
### Added
- metrics-cassandra-graphite.rb: Earlier versions of nodetool incorrectly append a `.` to the `ms` SI unit. In newer versions where this has been corrected, the missing `.` failed to match causing a missed `chomp` operation. (@zenmetsu)

### Removed
- metrics-cassandra-graphite.rb: removed superfluous gsub operation (@zenmetsu) (@majormoses)

## [2.0.2] - 2018-01-25
### Fixed
- metrics-cassandra-graphite.rb: fixed conditional assignments broken by agressive rubocop rule fix and following the instructions during a demo (@majormoses)

## [2.0.1] - 2018-01-23
### Changed
- no-op change (@majormoses)

## [2.0.0] - 2018-01-23
### Security
- updated `rubocop` dependency to `~> 0.51.0` per: https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-8418. (@majormoses)

### Breaking Changes
- in order to bring in new rubocop dependency we need to drop ruby 2.0 support as it is EOL and aligns with out support policy. (@majormoses)

### Changed
- updated Changelog guideline location (@majormoses)

## [1.1.0] 2017-07-26
### Added
- Test Ruby 2.4.1 (@thomasriley)
- metrics-cassandra-graphite.rb: Added key cache parsing for newer nodetool version (@jthunt)

## [1.0.0] - 2016-11-26
### Changed
- Update some metrics not shown due to new nodetool version.

### Added
- Ruby 2.3.0 support

### Removed
- Ruby 1.9.3 support

## [0.0.5] - 2016-08-16
### Changed
- Updated sensu-plugin dependency from `= 1.2.0` to `~> 1.2.0`

## [0.0.4] - 2015-08-04
### Changed
- general cleanup

## [0.0.3] - 2015-07-14
### Changed
- updated sensu-plugin gem to 1.2.0

## [0.0.2] - 2015-06-02
### Fixed
- added binstubs

### Changed
- removed cruft from /lib

## 0.0.1 - 2015-04-30
### Added
- initial release

[Unreleased]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/3.0.0...HEAD
[3.0.0]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/2.1.0...3.0.0
[2.1.0]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/2.0.2...2.1.0
[2.0.2]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/2.0.1...2.0.2
[2.0.1]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/2.0.0...2.0.1
[2.0.0]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/1.0.0...2.0.0
[1.0.0]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/0.0.5...1.0.0
[0.0.5]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/0.0.4...0.0.5
[0.0.4]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/0.0.3...0.0.4
[0.0.3]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/0.0.2...0.0.3
[0.0.2]: https://github.com/sensu-plugins/sensu-plugins-cassandra/compare/0.0.1...0.0.2
