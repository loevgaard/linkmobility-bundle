# Linkmobility Bundle

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Quality Score][ico-code-quality]][link-code-quality]

Symfony bundle that integrates the [Linkmobility PHP SDK](https://github.com/loevgaard/linkmobility-bundle) into Symfony.

## Installation

### Step 1: Download the bundle

Open a command console, enter your project directory and execute the
following command to download the latest stable version of this bundle:

```bash
$ composer require loevgaard/linkmobility-bundle
```

This command requires you to have Composer installed globally, as explained
in the [installation chapter](https://getcomposer.org/doc/00-intro.md)
of the Composer documentation.

### Step 2: Enable the Bundle

Then, enable the bundle by adding it to the list of registered bundles
in the `app/AppKernel.php` file of your project:

```php
<?php
// app/AppKernel.php

// ...
class AppKernel extends Kernel
{
    public function registerBundles()
    {
        $bundles = array(
            // ...
            new Loevgaard\LinkmobilityBundle\LoevgaardLinkmobilityBundle(),
        );

        // ...
    }

    // ...
}
```

### Step 3: Configure the bundle
```yaml
loevgaard_linkmobility:
    api_key: insert your api key
```

## Testing

``` bash
$ composer test
```

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v/loevgaard/linkmobility-bundle.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/loevgaard/linkmobility-bundle/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/loevgaard/linkmobility-bundle.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/loevgaard/linkmobility-bundle.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/loevgaard/linkmobility-bundle
[link-travis]: https://travis-ci.org/loevgaard/linkmobility-bundle
[link-scrutinizer]: https://scrutinizer-ci.com/g/loevgaard/linkmobility-bundle/code-structure
[link-code-quality]: https://scrutinizer-ci.com/g/loevgaard/linkmobility-bundle
[link-author]: https://github.com/loevgaard
