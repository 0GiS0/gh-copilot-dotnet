# mi-api-netcore

Este proyecto es una API creada con .NET Core. 

## Estructura del proyecto

El proyecto tiene la siguiente estructura:

- `Controllers/ValuesController.cs`: Controlador que maneja las rutas de la API para obtener, crear, actualizar y eliminar valores.
- `Models`: Directorio destinado a contener clases de modelo que representan los datos que la API manejará.
- `Properties/launchSettings.json`: Configuración de lanzamiento para la aplicación.
- `appsettings.Development.json` y `appsettings.json`: Archivos de configuración para la aplicación.
- `Program.cs`: Punto de entrada de la aplicación.
- `Startup.cs`: Configura los servicios y la tubería de solicitud de la aplicación.
- `mi-api-netcore.csproj`: Archivo de proyecto de .NET Core.

## Cómo ejecutar el proyecto

Para ejecutar el proyecto, siga estos pasos:

1. Abra una terminal en la raíz del proyecto.
2. Ejecute el comando `dotnet run`.

Esto iniciará la aplicación en `http://localhost:5000`.

## Cómo contribuir

Si desea contribuir al proyecto, haga un fork del repositorio, realice sus cambios y luego envíe un pull request. Asegúrese de que sus cambios sean claros y estén bien documentados.