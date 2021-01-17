# yii2-yup-post

##Yee CMS - Post Module

####Backend module for managing posts 

This module is part of Yee CMS (based on Yii2 Framework).

Post module lets you easily create posts on your site. 

Installation
------------

- Install [Yee Media Module](https://github.com/ciapistess/yii2-yee-media) if it is not installed yet.

- Either run

```
composer require --prefer-dist ciapistess/yii2-yup-post "~0.1.0"
```

or add

```
"yeesoft/yii2-yup-post": "~0.1.0"
```

to the require section of your `composer.json` file.

- Run migrations

```php
yii migrate --migrationPath=@vendor/ciapistess/yii2-yup-post/migrations/
```

Configuration
------
- In your backend config file

```php
'modules'=>[
	'post2' => [
		'class' => 'ciapistess\post\PostModule',
	],
],
```

Dashboard widget
-------  

You can use dashboard widget to display short information about recent activity in the module.

Add this code in your control panel dashboard to display widget:
```php
echo \ciapistess\post2\widgets\dashboard\Posts::widget();
```

Screenshots
-------  

[Flickr - Yee CMS Post Module](https://www.flickr.com/photos/134050409@N07/sets/72157656324703598)
