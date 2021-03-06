# Add pretty favicons to your Laravel application on the fly

[![Latest Version on Packagist](https://img.shields.io/packagist/v/lukasmu/laravel-favicon.svg?style=flat-square)](https://packagist.org/packages/lukasmu/laravel-favicon)
[![Build Status](https://img.shields.io/travis/lukasmu/laravel-favicon/main.svg?style=flat-square)](https://travis-ci.com/github/lukasmu/laravel-favicon)
[![Quality Score](https://github.styleci.io/repos/233151342/shield?branch=main)](https://github.styleci.io/repos/233151342)
[![Total Downloads](https://img.shields.io/packagist/dt/lukasmu/laravel-favicon.svg?style=flat-square)](https://packagist.org/packages/lukasmu/laravel-favicon)

This package can be used to quickly generate customized and high-quality favicons for your Laravel application. The images are generated on the fly for different platforms and display resolutions. Usage is super simple and just requires including a view in your templates (see below).

Please note that this package is based on [beyondcode/laravel-favicon](https://packagist.org/packages/beyondcode/laravel-favicon) but serves a completely different purpose. 

## Installation

You can install the package via composer:

```bash
composer require lukasmu/laravel-favicon
```

## Usage

To add the icons to your site include the view ```favicon::head``` in the head section of your blade view(s).

``` php
<!doctype html>
<html>

<head>
    <title>Example</title>
    @include('favicon::head')
    ...
</head>

<body>
...
</body>

</html>
```

## Customization

You can publish the config file with:

```bash
php artisan vendor:publish --provider="LukasMu\Favicon\FaviconServiceProvider" --tag="config"
```

Feel free to set the appropriate environmental variables (or edit the config file) in order to customize the favicons.

## Testing

You can run all tests via composer as well:

``` bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email [hello@lukasmu.com](hello@lukasmu.com) instead of using the issue tracker.

## Postcardware

You are free to use this package, but if it makes it to your production environment we highly appreciate you sending us a postcard from your hometown. The address is: Lukas Müller, Dirklangendwarsstraat 5, 2611HZ Delft, The Netherlands.

## License

The MIT License (MIT). Please see [LICENSE](LICENSE.md) for more information.
