yii2-ajaxcrud modify from JHONITVN
=============

Features
------------
+ Create, read, update, delete in onpage with Ajax
+ Bulk delete suport
+ Pjax widget suport
+ Export function(pdf,html,text,csv, excel,json)

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist origrata/yii2-ajaxcrud "@dev"
```

or add

```
"origrata/yii2-ajaxcrud": "^2.1"
```

to the require section of your `composer.json` file.


Usage
-----
For first you must enable Gii module Read more about [Gii code generation tool](http://www.yiiframework.com/doc-2.0/guide-tool-gii.html)

Because this extension used [kartik-v/yii2-grid](https://github.com/kartik-v/yii2-grid) extensions so we must config gridview module before

Let 's add into modules config in your main config file
```php
'modules' => [
    'gridview' =>  [
        'class' => \kartik\grid\Module::class,      
    ]       
]
```
Note: Font Awesome icons not required! See [Bootstrap icons](https://demos.krajee.com/grid#bootstrap-icons)!

You can then access Gii through the following URL:


 in param.php file add
 
 'bsVersion' => '5.x',

http://localhost/path/to/index.php?r=gii

and you can see <b>Ajax CRUD Generator</b>


Lets contibute to keep it updated and make it useful for all friends.
