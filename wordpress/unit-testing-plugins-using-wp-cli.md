# Unit testing WordPress plugin

In order to scaffold and run tests you need to have a `WP CLI` installed.

## Instructions

Go to the root of your project and install plugin scaffolding:

`wp scaffold plugin-tests my-plugin`

Then go to your plugin root and initialize testing environment:

`bash bin/install-wp-tests.sh wordpress_test root '' localhost latest`

(when using Vagrant I need to initialize testing enviroment each time after i stop and start the machine)

## Extras

Visit [WP plugin unit tests handbook](https://make.wordpress.org/cli/handbook/plugin-unit-tests/) for more details and settings.
