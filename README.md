# MarsBased Circle CI project configuration

This repository has the required Circe CI configuration to the MarsBased Projects. It is configured to work on Rails applications that:
* Use RSpec.
* Use `:selenium_chrome_headless` as the Javascript driver to run system tests.
* Use Yarn to manage front-end dependencies. 

If your application has a different setup, you will need to adapt the `.circleci/config.yml` file as needed.

## Add configuration to an application

* execute the following command in your application's root path: `source <(curl https://raw.githubusercontent.com/MarsBased/circleci/master/bin/initialize)`
* Add `gem 'rspec_junit_formatter', require: false` in the `:development` group of your Gemfile.
