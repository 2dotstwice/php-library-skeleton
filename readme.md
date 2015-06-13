A skeleton for PHP library projects.

# Setup your project

Copy over all files - except this readme - to your new PHP project and modify
the following parts to your needs:

- composer.json:
  - [name]
  - [description]
  - [license] if Apache-2.0 is not desired
  - [authors]
  - PHP namespace prefixes in [autoload] and [autoload-dev]
- build.xml
  - [project name][Phing project name]
- .travis.yml
  - [e-mail notification recipients][Travis CI e-mail notifications]

Run `composer install`.

Put your classes in the src directory, and PHPUnit tests in the tests directory. 
Follow the [PSR-4] conventions for autoloading and [PSR-2] conventions for coding
style.

Run a full test (lint check, coding standards check and unit tests) with 
`./vendor/bin/phing test`.

# Setup third-party services

Register your project on:

- [Travis CI]
- [Coveralls]
- [Packagist]


[name]: https://getcomposer.org/doc/04-schema.md#name
[description]: https://getcomposer.org/doc/04-schema.md#description
[license]: https://getcomposer.org/doc/04-schema.md#license
[authors]: https://getcomposer.org/doc/04-schema.md#authors
[autoload]: https://getcomposer.org/doc/04-schema.md#psr-4
[autoload-dev]: https://getcomposer.org/doc/04-schema.md#autoload-dev
[Phing project name]: https://www.phing.info/docs/guide/trunk/ch04s02.html
[Travis CI e-mail notifications]: http://docs.travis-ci.com/user/notifications/#Email-notifications
[PSR-4]: http://www.php-fig.org/psr/psr-4/
[PSR-2]: http://www.php-fig.org/psr/psr-2/
[Travis CI]: https://travis-ci.org/
[Packagist]: https://packagist.org/
[Coveralls]: https://coveralls.io/
