Nitrapi-PHP
===========
[![PHP version](https://badge.fury.io/ph/nitrado%2Fnitrapi-php-lib.svg)](http://badge.fury.io/ph/nitrado%2Fnitrapi-php-lib)

PHP based SDK for the Nitrapi RESTful API.


Recommends
---------

* PHP 5.4 or higher
* Composer


Installation
------------

Edit the composer.json and execute composer.phar update
``` php
{
    "require": {
        "nitrado/nitrapi-php-lib": "dev-master",
    }
}
```

Example
-------

```php
<?php

require_once '../vendor/autoload.php';

try {
    $api = new \Nitrapi\Nitrapi("<accesss token>");
    
    var_dump($api->getServices());
    
} catch(\Exception $e) {
    var_dump("API Error: " . $e->getMessage());
}
```
