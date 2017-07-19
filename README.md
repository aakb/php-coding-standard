# ITK PHP CodeSniffer Coding Standard

A coding standard to check against the [Symfony coding standards](http://symfony.com/doc/current/contributing/code/standards.html), originally shamelessly copied from the -disappeared- opensky/Symfony2-coding-standard repository.

Based on https://packagist.org/packages/escapestudios/symfony2-coding-standard

## Installation

### Composer

This standard can be installed with the [Composer](https://getcomposer.org/) dependency manager.

1. [Install Composer](https://getcomposer.org/doc/00-intro.md)

2. Setup repositry in composer.json

				"repositories": [
		        {
		            "type": "vcs",
		            "url": "git@github.com:aakb/php-coding-standard.git"
		        }
		    ],

3. Install the coding standard as a dependency of your project

        composer require --dev aakb/php-coding-standard:~1.0

4. Add the coding standard to the PHP_CodeSniffer install path

        vendor/bin/phpcs --config-set installed_paths vendor/aakb/php-coding-standard

5. Check the installed coding standards for "Symfony"

        vendor/bin/phpcs -i

6. Done!

        vendor/bin/phpcs /path/to/code
