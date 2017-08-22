# 

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Total Downloads][ico-downloads]][link-downloads]


## Install

Via Composer

``` bash
$ composer require ahmadarif/terbilang
```

## Usage

``` php
$teks = Terbilang::make(1000086);
```

Then add the service provider in `config/app.php`:

```php
AhmadArif\Terbilang\TerbilangServiceProvider::class,
```

And then, add the facade of this package to the $aliases array:

```php
'Terbilang' => AhmadArif\Terbilang\Facade\Terbilang::class,
```

## Usage

```php
Route::get('/', function () {
    return Terbilang::convert(34124);
});
```

or

```php
Route::get('/', function () {
    return Terbilang::convert('34124');
});
```

## Security

If you discover any security related issues, please email ahmad.arif019@gmail.com instead of using the issue tracker.

## Credits

- [Ahmad Arif][link-author]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v//.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt//.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/ahmadarif/terbilang
[link-downloads]: https://packagist.org/packages/ahmadarif/terbilang
[link-author]: https://github.com/ahmadarif
