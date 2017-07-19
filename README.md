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

4. Add setup scripts to composer.json.

		 		"scripts": {
		        "post-install-cmd": [
		            "vendor/bin/phpcs --config-set installed_paths vendor/aakb/php-coding-standard",
		            "ln -s vendor/aakb/php-coding-standard/hooks/pre-commit .git/hooks/pre-commit"
		        ]
		    }

3. Install the coding standard as a dependency of your project

        composer require --dev aakb/php-coding-standard:~1.0

### Manual install.

1. Add the coding standard to the PHP_CodeSniffer install path

        vendor/bin/phpcs --config-set installed_paths vendor/aakb/php-coding-standard

2. Add pre-commit hook.

				ln -s vendor/aakb/php-coding-standard/hooks/pre-commit .git/hooks/pre-commit

2. Check the installed coding standards for "Symfony"

        vendor/bin/phpcs -i

3. Done!

        vendor/bin/phpcs /path/to/code

