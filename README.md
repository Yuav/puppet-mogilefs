# Puppet module: mogilefs

This is a Puppet module for mogilefs.

Released under the terms of Apache 2 License.


## USAGE - Basic management

* Install mogilefs with default settings

        class { 'mogilefs': }

* Install a specific version of MogileFS::Server package

        class { 'mogilefs':
          version => '2.67',
        }

* Remove mogilefs package

        class { 'mogilefs':
          absent => true
        }

* Enable auditing without without making changes on existing mogilefs configuration *files*

        class { 'mogilefs':
          audit_only => true
        }

* Module dry-run: Do not make any change on *all* the resources provided by the module

        class { 'mogilefs':
          noops => true
        }


## TESTING
[![Build Status](https://travis-ci.org/Yuav/puppet-mogilefs.png?branch=master)](https://travis-ci.org/Yuav/puppet-mogilefs)

