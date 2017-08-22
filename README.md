# Terbilang Laravel

[![Release Version](https://img.shields.io/github/release/ahmadarif/terbilang-laravel.svg)](https://github.com/ahmadarif/laravel-terbilang/releases)
[![License](https://poser.pugx.org/ahmadarif/terbilang/license)](https://packagist.org/packages/ahmadarif/terbilang)
[![Total Downloads](https://poser.pugx.org/ahmadarif/terbilang/downloads)](https://packagist.org/packages/ahmadarif/terbilang)


## Install

Via Composer

``` bash
$ composer require ahmadarif/terbilang
```

## Usage

Add the service provider in `config/app.php`:

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

- [Ahmad Arif](https://packagist.org/packages/ahmadarif/terbilang/stats)


## Base Project

Thanks to [Mulia Nasution](https://github.com/mul14/terbilang-php), as the basic project for the creation of this library.


## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.