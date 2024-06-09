
# Tutorial laravel filament






## Buat database di laragon atau xamp
- http://localhost/phpmyadmin/index.php?route=/server/databases
- create database sesuai nama project

## Instal laravel terlebih dahulu

 - [dokumentasi laravel](https://laravel.com/docs/10.x)

## perintah di terminal membuat framework laravel
```bash
composer create-project laravel/laravel:^10.0 example-app
```
## Setting env agar tersambung database
```bash
DB_CONNECTION=mysql //DB_CONNECTION di mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=latihan // merupakan database yang dibuat di mysql
DB_USERNAME=root
DB_PASSWORD=
```

```bash
composer create-project laravel/laravel:^10.0 example-app
```

- perintah migrasi data ke database
```bash
php artisan migrate
```
- run project laravel
```bash
php artisan serve
```
- Install Filament UI for admin panel:
```bash
composer require filament/filament:"^3.2" -W
```

- Set up Filament UI:
```bash
php artisan filament:install --panels
php artisan make:filament-user
```

- install sidebar filament
```bash
php artisan make:filament-resource Customer
```

