## New Relic Varnish Extension

### Instructions for running the Varnish extension agent

1. Go to [the tags list](https://github.com/varnish/newrelic_varnish_plugin/tags) and find the latest tar.gz
2. Download and extract the source
3. run `bundle install` to install required gems
4. Copy `config/template_newrelic_plugin.yml` to `config/newrelic_plugin.yml`
5. Edit `config/newrelic_plugin.yml` and replace "YOUR_LICENSE_KEY_HERE" with your New Relic license key
6. Edit the `config/newrelic_plugin.yml` if you are running Varnish
   with an -n argument or if you want to connect to a remote instance
7. Execute `./newrelic_varnish_plugin`
8. Go back to the Extensions list and after a brief period you will see an entry for your extension

## Connecting to a remote instance

The connection is done by executing varnishstat remotely via ssh, so be sure to add the public key of the user running the process 
in the authorized_keys file usually located in `/home/[user]/.ssh/authorized_keys` in the remote server for the configured user.