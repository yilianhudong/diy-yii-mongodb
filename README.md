DIY Yii PHP Framework
===========================

This is the core framework code of [Yii 2](https://github.com/yiisoft/yii2#readme).

This repository is a read-only git subsplit of <https://github.com/yiisoft/yii2>.
Please submit issue reports and pull requests to the main repository.
For license information check the [LICENSE](LICENSE.md)-file.

Installation
------------

The preferred way to install the Yii framework is through [composer](http://getcomposer.org/download/).

Either run

```
composer require yilianhudong/diy-yii-mongodb
```

or add

```json
"yilianhudong/diy-yii-mongodb": "~1.0.0",
```

to the require section of your composer.json.

Configuration
-------------

To use this extension, simply add the following code in your application configuration:

```php
return [
    //....
    'components' => [
        'mongodb' => [
            'class' => '\yii\mongodb\Connection',
            'dsn' => 'mongodb://@localhost:27017/mydatabase',
            'options' => [
                "username" => "Username",
                "password" => "Password"
            ]
        ],
    ],
];