# laravel
Instrucciones para la instalacion de un proyecto base con Laravel

## Instalar Laravel

```
composer create-project laravel/laravel .
```

## Actualizar paquete de idiomas

```
composer require "overtrue/laravel-lang:~5.0"
```

Reemplazar locate en el archivo config/app.php

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

## Instalar LiveWire
```
php artisan jetstream:install livewire
```

## Actualizar Mix
```
npm install && npm run dev
```

## Ejecutar migraciones

Actualizar la configuracion de la base en el archivo .dev
Por defecto, poner en todo laravel

```
php artisan migrate:fresh
```

## Modificar permisos de ficheros
```
chmod 777 storage/ -R
```
```
chmod 777 bootstrap/ -R
```

## Instalar gestor gráfico de migraciones
```
composer require rezaamini-ir/migrator --dev
```

Se usa misitio.desa/migrator

