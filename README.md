

### Usando el archivo
En la raíz de su aplicación, cree una carpeta de ajustes preestablecidos .
- Descargue un archivo del repositorio y descomprímalo.
- https://github.com/laravel-frontend-presets/argon/archive/master.zip 
- Copie y pegue la carpeta argon-master en ajustes preestablecidos (creada en el paso 2) y cámbiele el nombre a argon
- Abrir composer.jsonarchivo
- Añadir "LaravelFrontendPresets\\ArgonPreset\\": "presets/argon/src"a autoload/psr-4y aautoload-dev/psr-4
- Agregar LaravelFrontendPresets\ArgonPreset\ArgonPresetServiceProvider::classal config/app.phparchivo
- Escriba en su terminal: composer require laravel/uiyphp artisan ui vue --auth
- En tu terminal ejecutacomposer dump-autoload
- Ejecute php artisan ui argonel comando para instalar el ajuste preestablecido de Argon. Esto instalará todos los
- activos necesarios y también las vistas de autenticación personalizadas, también agregará la ruta de autenticación
- routes/web.php(NOTA: si ejecuta este comando varias veces, asegúrese de limpiar las entradas de autenticación 
- duplicadas en rutas/web.php)
- Ejecutar php artisan migrate --seedpara crear una tabla de usuarios básicos.