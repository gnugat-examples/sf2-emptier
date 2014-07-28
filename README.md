# Symfony2 Emptier Edition

Does the [Symfony Standard Edition](http://symfony.com/distributions) contains
too many things you'll never use?

Then start your projects with this distribution:

    composer create-project gnugat/sf2-emptier <vendor>

**Note**: `<vendor>` is to be replace with the project's name.

Next you'll have to configure the project specific parameters:

    cp app/config/parameters.yml.dist app/config/parameters.yml

Don't forget to edit `app/config/parameters.yml` and change the value of the
`secret` parameter.

You might also want to change the `composer.json`'s  `name`, `license` and
`description` parameters.

Finally remove the content of this `README.md` file and replace it with your
own.

## Features

Here's the list of dependencies:

* [FrameworkBundle](https://github.com/symfony/FrameworkBundle)

Here's the role of the files you'll likely edit:

* `app/config/config.yml`: common configuration
* `app/config/config_prod.yml`: configuration only found in production
* `app/config/config_test.yml`: configuration only used in tests
* `app/config/parameters.yml`: sensitive configuration (passwords, etc)
* `app/config/routing.yml`: linking controllers to URLs
* `app/AppKernel.php`: where you register new bundles
