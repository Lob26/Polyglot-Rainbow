# LARAVEL
# Estructura
```
project-root/
|-- app/
|   |-- Console/
|       |-- Commands/
|   |-- Http/
|       |-- Controllers/
|           |-- ReportController.php
|       |-- Middleware/
|       |-- Requests/
|       |-- Resources/
|           |-- views/
|-- database/
|   |-- migrations/
|-- routes/
|   |-- web.php
|-- resources/
|   |-- views/
|-- composer.json
|-- artisan
```
# Modelo
```php
// En app/Statistic.php (por ejemplo)

namespace App;

use Illuminate\Database\Eloquent\Model;

class Statistic extends Model
{
    // Define los campos y métodos según sea necesario
}
```
# To learn
- Laravel
- Migraciones en Laravel
- Eloquent ORM
- Blade Templating Engine
- Artisan Console
- Controladores y Rutas en Laravel
- Middleware en Laravel
- Manejo de Datos Estadisticos
- Composer
- Principios de Seguridad
