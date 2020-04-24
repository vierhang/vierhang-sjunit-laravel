<h1 align="center"> junit-laravel </h1>

<p align="center"> A simplified version of the laravel framework unit test.</p>

## 框架要求

Laravel >= 5.1

## 安装

```shell
$ composer require vierhang/junit-laravel
```

## 配置

Laravel应用

在 `config/app.php` 注册 ServiceProvider 和 Facade (Laravel 5.5 无需手动注册)

'providers' => [ 
	Vierhang\JunitLaravel\Providers\SJunitServiceProvider::class,
]

然后在浏览器中直接访问路由

Route::get('/', 'SJunitController@index'); 
Route::post('/', 'SJunitController@store')->name('junit.store');

## License

MIT