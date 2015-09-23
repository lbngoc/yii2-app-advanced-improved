Improved Yii 2 Advanced Project Template
========================================

[![Latest Stable Version](https://poser.pugx.org/mghollander/yii2-app-advanced-improved/v/stable)](https://packagist.org/packages/mghollander/yii2-app-advanced-improved)
[![Total Downloads](https://poser.pugx.org/mghollander/yii2-app-advanced-improved/downloads)](https://packagist.org/packages/mghollander/yii2-app-advanced-improved)
[![Latest Unstable Version](https://poser.pugx.org/mghollander/yii2-app-advanced-improved/v/unstable)](https://packagist.org/packages/mghollander/yii2-app-advanced-improved)
[![License](https://poser.pugx.org/mghollander/yii2-app-advanced-improved/license)](https://packagist.org/packages/mghollander/yii2-app-advanced-improved)

Improved Yii 2 Advanced Project Template is an expented version of [Yii 2 Advanced Project Template](https://github.com/yiisoft/yii2-app-advanced).

I have:
- added `chmod` to the `init` for all dirs Gii can write in
- added an staging environment to the `init`
- separeted db configurations from `main-local.php`
- added `*-local.php` to all `config/.gitignore` files
- added pretty URLs to backend and frontend configs
- added `.htaccess` to all `web/.gitignore` files (incase you need them)


Installing using Composer
-------------------------

If you do not have [Composer](http://getcomposer.org/), follow the instructions in the
[Installing Yii](https://github.com/yiisoft/yii2/blob/master/docs/guide/start-installation.md#installing-via-composer) section of the definitive guide to install it.

With Composer installed, you can then install the application using the following commands:

    composer global require "fxp/composer-asset-plugin:~1.0.3"
    composer create-project --prefer-dist mghollander/yii2-app-advanced-improved yii-application

After installing the application you need to add your db config to `common/config/db-local.php`

```
<?php
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=localhost;dbname=yii2-advanced',
    'username' => 'root',
    'password' => '',
    'charset' => 'utf8',
];
```
Now follow the Yii 2 Advanced Project [Template Application preparation steps](https://github.com/yiisoft/yii2-app-advanced/blob/master/docs/guide/start-installation.md#preparing-application)