## New Relic Varnish Extension

This is a fork of [the original](https://github.com/varnish/newrelic_varnish_plugin) which no longer seems to be maintained

This runs on the Varnish server and reports the values from
varnishstat back into New Relic.

## Instructions for running the Varnish extension agent

1. Check out the latest source from develop
2. run `bundle install` to install required gems
3. Copy `config/template_newrelic_plugin.yml` to path of your choise, ex `/etc/newrelic/newrelic_varnish_plugin.yml`
4. Edit the `newrelic_plugin.yml` copy you just made and replace "YOUR_LICENSE_KEY_HERE" with your New Relic license key
5. Edit the configuration further if you are running Varnish with an -n argument
6. Execute `./newrelic_varnish_plugin -h` for usage instructions
7. Go back to the Extensions list and after a brief period you will see an entry for your extension
