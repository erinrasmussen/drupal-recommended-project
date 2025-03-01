Acquia Drupal Recommended Project
====

This is a project template providing a great out-of-the-box experience for new
Drupal 10 projects hosted on Acquia. It is based on the [Drupal Recommended
Project](https://github.com/drupal/recommended-project/tree/9.0.x), with the
principal difference being the addition of several modules and packages that
provide the best possible out-of-the-box experience for Acquia customers.

This project includes the following packages and configurations:
* [Drupal core](https://www.drupal.org/project/drupal)
* [Drupal core scaffold](https://www.drupal.org/docs/develop/using-composer/using-drupals-composer-scaffold)
* [Acquia CMS](https://github.com/acquia/acquia-cms-starterkit) (Starter kit)
* [Drupal Recommended Settings](https://github.com/acquia/drupal-recommended-settings)
* [Drush](https://github.com/drush-ops/drush) (Drupal CLI and development tool)
* [Asset Packagist](https://asset-packagist.org/) repository, package, and configuration
* [Acquia environment detection](https://github.com/acquia/drupal-environment-detector)
* [Acquia platform memcache settings](https://github.com/acquia/memcache-settings)
* Best practices for Drupal development, testing and project architecture

The Acquia CMS Starterkit allows you to install Drupal for a given style of CMS:

| Name  | Description |
| ------------- | ------------- |
| Acquia CMS Enterprise Low-code  | The low-code starter kit will install Acquia CMS with Site Studio and a UIkit. It provides drag and drop content authoring and low-code site building. An optional content model can be added in the installation process.  |
| Acquia CMS Community  | The community starter kit will install Acquia CMS. An optional content model can be added in the installation process.  |
| Acquia CMS Headless  | The headless starter kit preconfigures Drupal for serving structured, RESTful content to 3rd party content displays such as mobile apps, smart displays and frontend driven websites (e.g. React or Next.js).  |

For more information on selecting the Acquia CMS Starterkit that best fits your
use case follow
[instructions](https://docs.acquia.com/acquia-cms/install-cms).

## Installation

Create a new project using Composer:
```
composer create-project --no-interaction acquia/drupal-recommended-project
```

Once you create the project, you can and should customize `composer.json` and
the rest of the project to suit your needs. You will receive updates from any
dependent packages, but not from the project template itself. It's yours to
keep!

For instance, you can remove a provided package by running the following command
 and committing the changed `composer.json` and `composer.lock` to Git:
```
composer remove acquia/mysql56
```

You should only commit changes to `composer.json` and `composer.lock`. Do not
commit files in the `vendor`, `docroot/core`, and similar directories (these are
   ignored by the provided `.gitignore` file). In order to run your application
   in another environment, you’ll need to run `composer install` to reinstall
   these assets. [Acquia Code Studio’s](https://docs.acquia.com/code-studio/)
   Auto DevOps feature can do this automatically when deploying to Acquia Cloud.

## Usage (Install Acquia CMS)

Install Acquia CMS using starterkit follow
[instructions](https://docs.acquia.com/acquia-cms/using-split-commands).


## Other Drupal versions

Drupal 11 is installed by default. To install Drupal 10, use the below command:
```
composer create-project acquia/drupal-recommended-project:^2
```
To install Drupal 9, use the below command:
```
composer create-project acquia/drupal-recommended-project:^1
```

## Next steps

After creating your project, if you'd also like to use Acquia BLT, do the
following:
* Add BLT via Composer with `composer require acquia/blt`
* Install the [BLT Launcher](https://github.com/acquia/blt-launcher) and follow
the rest of the
[BLT setup guide](https://docs.acquia.com/blt/install/next-steps/).
* Set up automated testing using BLT recipes and plugins such as
[BLT Behat](https://github.com/acquia/blt-behat) and the
[Acquia Drupal Spec Tool](https://github.com/acquia/drupal-spec-tool).

# License

Copyright (C) 2023 Acquia, Inc.

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License version 2 as published by the Free
Software Foundation.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.
