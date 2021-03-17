# Laravel User Command

[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE)

Create a user with artisan command. 

**NEW:** Added support for php ^7.3 or ^8.0 and Laravel 8

## Install
Install via composer
```
composer require rap2hpoutre/create-user-command
```
Add the Create User command to `app/Console/Kernel.php` in protected `$commands` array
```php
\Andp97\CreateUser\Command::class,
```

## Usage

Define fillable attributes in your `User` class.

```
protected $fillable = ['name', 'email', 'role'];
```

Then, run `user:create` command.

![demo](demo.gif)

## Why

Sometimes, I have to manually create user (with no web interface).
