# laravel
Instrucciones para la instalacion de un proyecto base con Laravel

## Instalar Laravel

```
composer create-project laravel/laravel .
```

### Actualizar paquete de idiomas

```
composer require "overtrue/laravel-lang:~5.0"
```

Reemplazar locate en el archivo config/app.php

## Instalar JetStream

```
composer require laravel/jetstream
```

### Instalar LiveWire
```
php artisan jetstream:install livewire
```

### Actualizar Mix
```
npm install && npm run dev
```

## Ejecutar migraciones

Actualizar la configuracion de la base en el archivo .dev
Por defecto, poner en todo laravel

```
php artisan migrate:fresh
```
