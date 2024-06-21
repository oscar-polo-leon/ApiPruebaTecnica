# API REST en .NET

Este proyecto es una API REST construida con .NET. La siguiente guía te ayudará a configurar y ejecutar el proyecto en tu entorno local.

## Pasos para Configurar y Ejecutar el Proyecto

### 1. Clonar el Repositorio

Primero, clona el repositorio en tu máquina local usando el siguiente comando:

```bash
git clone https://github.com/oscar-polo-leon/ApiPruebaTecnica.git
```
### 2. Abrir la Solución

Abre la solución .sln en tu IDE preferido. Puedes hacerlo desde la línea de comandos o directamente desde el menú de tu IDE.

### 3. Modificar la Propiedad "dev" del appsettings.json
En el archivo appsettings.json busca la sección "ConnectionStrings" y cambia el valor de "dev" por el string de conexión de tu base de datos.
```bash
"ConnectionStrings": {
    "dev": "Data Source = DESKTOP; Initial Catalog = CHOUCAIRTESTING_PRUEBATECNICA; Trusted_Connection = True; MultipleActiveResultSets = true; TrustServerCertificate = true"
  }
```
### 4. Crear la base de datos 
En sql server crear la base de datos.
```bash
CHOUCAIRTESTING_PRUEBATECNICA
```
### 5. Crear la base de datos 
Desde la consola powershell en visual studio ejecutar los siguiente comando.
```bash
Add-Migration AddDescriptionToProduct
Update-Database
```
### 6. Ejecutar y Probar en Swagger o desde un cliente
