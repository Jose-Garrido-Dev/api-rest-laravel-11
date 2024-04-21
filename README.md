<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

partimos con crear proyecto laravel 11
php artisan install:api para crear la ruta de api en routes

php artisan make:migration  create_student_table    para crear tabla estudiantes con la cual consumiremos el api

en la migración creamos los siguientes campos
        Schema::create('student', function (Blueprint $table) {
            $table->id();
            $table->string('name');
            $table->string('email');
            $table->string('phone');
            $table->string('languaje');
            $table->timestamps();
        });

Posteriormente creamos el modelo para interactuar con la base de datos

php artisan make:model Student

php artisan make:controler studentController


se crea el crud en el controlador para realizar la api 

La base de datos utilizada es sqlite, pero de igual manera puedes utilizar el .env y usar mysql o la que estimes conveniente.



