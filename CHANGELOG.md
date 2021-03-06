## 1.0.0.alpha.6 / 2013-05-08

### New features

* Pull request [#77][]: Support encrypted data bag secrets ([@arunthampi][])
* Issue [#92][]: Support single cookbook with no dependencies and no Berksfile. ([@fnichol][])

### Bug fixes

* Fix Omnibus installation on nodes using plain sh (vs. bash). ([@fnichol][])

### Improvements

* Issue [#84][]: Fix `kitchen list` heading alignment. ([@fnichol][])


## 1.0.0.alpha.5 / 2013-04-23

### Improvements

* Pull request [#81][]: Clean up error reporting in CLI output. ([@fnichol][])
* Pull request [#76][]: Swap out shell-based kb for Ruby-based Busser gem. ([@fnichol][])
* Pull request [#82][], issue [#61][]: Install Omnibus package via either wget or curl. ([@fnichol][])
* Catch YAML data merging errors as user errors. ([@fnichol][])
* Issue [#80][]: Add a more helpful error message when a driver could not be loaded. ([@fnichol][])


## 1.0.0.alpha.4 / 2013-04-10

### Bug fixes

* #get_all_instances must return actors in parallel mode in CLI. ([@fnichol][], [@bryanwb][]).

### Improvements

* Refactor `kitchen plugin create` to drop Bundler dependency completely. ([@fnichol][])


## 1.0.0.alpha.3 / 2013-04-05

### Bug fixes

* Fix :require_chef_omnibus driver_config option to eliminate re-installation ([@fnichol][])
* Remove implicit Bundler dependency in `kitchen init`. ([@fnichol][])

### New features

* Add --auto-init flag to `kitchen test` (default: false) ([@fnichol][])

### Improvements

* Update base box URLs. ([@fnichol][])
* Extract .kitchen.yml to an ERB template & update box URLs. ([@fnichol][])
* Add more spec coverage. ([@fnichol][])


## 1.0.0.alpha.2 / 2013-03-28

### Bug fixes

* Remove catch-all rescue in Driver.for_plugin (reason provided in commit message). ([@fnichol][])

### New features

* Add --log-level flag to CLI for test, create, converge, setup, verify, destroy, and login actions. The environment variable `KITCHEN_LOG` may still be used to also set the logging level. ([@fnichol][])
* Driver::SSHBase and subclass drivers now support setting a :port number in .kitchen.yml or in instance state. ([@fnichol][])

### Improvements

* Support thor 0.16.0 and 0.17.0+. ([@fnichol][])
* Support SSH config from #state & #config in Driver::SSHBase, helping drivers such as kitchen-vagrant. ([@fnichol][])


## 1.0.0.alpha.1 / 2013-03-22

### Bug fixes

* Support (and test) for Rubygems 2.0.x and 1.8.x. ([@fnichol][])

### New features

* Pull request [#71][]: Updates to `kitchen init` to be non-interactive (add `--driver` flag), add subcommand support, and introduce `kitchen driver discover`. ([@fnichol][])
* Add `Driver#verify_dependencies` to be invoked once when Driver is loaded. ([@fnichol][])

### Improvements

* Pull request [#73][]: [Breaking] Modify `ShellOut#run_command` to take an options Hash. ([@fnichol][])
* Add :quiet option on `ShellOut#run_command`. ([@fnichol][])
* [Breaking] `Driver#login_command` returns a Driver::LoginCommand object. ([@fnichol][])
* Pull request [#74][]: Switch driver alias (-d) to (-D) in Init generator ([@reset][])
* Pull request [#64][]: Make `require_chef_omnibus: true` safe. ([@mattray][])
* Pull request [#65][]: Fix for line length and style (tailor). ([@ChrisLundquist][])


## 1.0.0.alpha.0 / 2013-03-02

The initial release.

<!--- The following link definition list is generated by PimpMyChangelog --->
[#61]: https://github.com/opscode/test-kitchen/issues/61
[#64]: https://github.com/opscode/test-kitchen/issues/64
[#65]: https://github.com/opscode/test-kitchen/issues/65
[#71]: https://github.com/opscode/test-kitchen/issues/71
[#73]: https://github.com/opscode/test-kitchen/issues/73
[#74]: https://github.com/opscode/test-kitchen/issues/74
[#76]: https://github.com/opscode/test-kitchen/issues/76
[#77]: https://github.com/opscode/test-kitchen/issues/77
[#80]: https://github.com/opscode/test-kitchen/issues/80
[#81]: https://github.com/opscode/test-kitchen/issues/81
[#82]: https://github.com/opscode/test-kitchen/issues/82
[#84]: https://github.com/opscode/test-kitchen/issues/84
[#92]: https://github.com/opscode/test-kitchen/issues/92
[@ChrisLundquist]: https://github.com/ChrisLundquist
[@arunthampi]: https://github.com/arunthampi
[@bryanwb]: https://github.com/bryanwb
[@fnichol]: https://github.com/fnichol
[@mattray]: https://github.com/mattray
[@reset]: https://github.com/reset
