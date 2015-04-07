## sensu-plugins-cassandra

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-cassandra.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-cassandra)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-cassandra.svg)](http://badge.fury.io/rb/sensu-plugins-cassandra)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-cassandra/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-cassandra)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-cassandra/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-cassandra)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-cassandra.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-cassandra)

## Functionality

## Files
 * bin/check-cassandra-schema
 * bin/metrics-cassandra-graphite

## Usage

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-cassandra -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-cassandra`

#### Bundler

Add *sensu-plugins-cassandra* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-cassandra' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-cassandra' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
