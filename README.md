# laravel
Instrucciones para la instalacion de un proyecto base con Laravel

## Instalar Laravel

```
composer create-project laravel/laravel .
```

## Modificar permisos de ficheros
```
chmod 777 storage/ -R && chmod 777 bootstrap/ -R
```

## Ejecutar migraciones

Actualizar la configuracion de la base en el archivo .dev
Por defecto, poner en todo laravel

```
php artisan migrate:fresh
```

## Actualizar paquete de idiomas

```
composer require "overtrue/laravel-lang:~5.0"
```

Reemplazar locate en el archivo config/app.php

## Instalar LiveWire
```
composer require livewire/livewire
```

## Instalar Parsedown
```
composer require erusev/parsedown
```

## Instalar visor web de rutas
```
composer require garygreen/pretty-routes --dev
```
Se usa misitio.desa/routes

composer require garygreen/pretty-routes
## Instalar gestor gráfico de migraciones
```
composer require rezaamini-ir/migrator --dev
```
Se usa misitio.desa/migrator

## Instalar barra de desarrollo
```
composer require barryvdh/laravel-debugbar --dev
```

## Instalar API
```
composer require cloudcreativity/laravel-json-api

composer require --dev "cloudcreativity/json-api-testing"
```

## Instalar JetStream

```
composer require laravel/jetstream
```

Si se quiere habilitar las fotos de perfil, hay que editar el archivo config/jetstream y desmarcar la opcion. 
Despues, hay que ejecutar
```
php artisan storage:link
```

Si se quiere quitar la validacion de dos factores, el registro de nuevos usuarios u otras configuraciones de ingreso, hay que editar el archivo config/fortify y desmarcar la opcion correspondiente. 

## Actualizar Mix
```
npm install && npm run dev
```

