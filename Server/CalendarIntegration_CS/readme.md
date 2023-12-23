# ASP.NET
# Estructura
```
project-root/
|-- CalendarIntegration/
|   |-- Controllers/
|       |-- CalendarController.cs
|   |-- Models/
|       |-- TaskEvent.cs
|   |-- Services/
|       |-- CalendarService.cs
|-- CalendarIntegration.sln
```
# Modelo
```csharp
public class TaskEvent
{
    public int Id { get; set; }
    public string Title { get; set; }
    public DateTime Deadline { get; set; }
    // Otros campos según sea necesario
}
```
# To learn
- ASP.NET Core
- Controladores y Rutas
- MVC
- Inyeccion de Dependencias
- Servicios
- Entity Frameworkd Core
- Trabajando con Fechas y Tiempos {-DateTime -TimeSpan}
- API RESTful
- Seguridad y Autorizacion
