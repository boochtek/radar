Rails Radar
===========

* Replace `YAML.load_file` with `Rails.application.config_for`
    * Since Rails 4.2
    * https://www.justinweiss.com/articles/the-lesser-known-features-in-rails-4-dot-2/
* Use [Rack Attack](https://github.com/kickstarter/rack-attack) middleware
* Use [fuubar](https://github.com/thekompanee/fuubar) formatter with RSpec
    * Outputs a progress bar
* Consider using the `--fail-fast` option to RSpec (when appropriate)
* Try using [paraspec](https://github.com/paraspec/paraspec ) instead of parallel_specs
* [Draper](https://github.com/drapergem/draper) - presenter objects
* SimpleForm or Formtastic
* [Pundit](https://github.com/varvet/pundit) for authorization
* [Rolify](https://github.com/RolifyCommunity/rolify) to define and manage roles
* Database cleaner gem for testing
* Shoulda matchers?
* Rails_best_practices gem
* RubyCritic
* Brakeman
* [Mina](https://github.com/mina-deploy/mina) for deployment
    * Faster than Capistrano, because it uses a single SSH connection, instead of per command
    * Does not have rollback yet
* [Ransack](https://github.com/activerecord-hackery/ransack) - build complex search forms
* Consider new alternative HTTP servers, instead of Puma
    * [Falcon](https://github.com/socketry/falcon)
    * [Iodine](https://github.com/boazsegev/iodine)
    * [Agoo](https://github.com/ohler55/agoo)
