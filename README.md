# Reto-Tecnico
Visualiza la Aplicación Web
https://reto-tecnico-aplicacion.herokuapp.com/Producto/Index

# Credenciales
 Usuario: mario@gmail.com
 Contraseña: @Mario123

# Creación de proyecto
dotnet new mvc -au Individual
Agregar la cadena de conexión
Modificar el Startup

# Creación de la migraciones
Eliminamos los 3 archivos que aparecen en Migrations
Instalamos el paquete de Npgsql.EntityFrameworkCore.PostgreSQL https://www.nuget.org/packages/Npgsql.EntityFrameworkCore.PostgreSQL/3.1.4
Instalamos el dotnet -ef https://docs.microsoft.com/en-us/ef/core/cli/dotnet
Ejecutamos la siquiente instrucción : dotnet ef migrations add CreateIdentitySchema --context El nombre de la carpeta donde esta alojado el proyecto.Data.ApplicationDbContext -o "Ubicación de la carpeta Migrations"
dotnet ef update database
Ejecutamos el proyecto
Aplicar Migrations

# Instalar Paquetes
https://www.nuget.org/packages/dotnet-aspnet-codegenerator/3.1.4

https://www.nuget.org/packages/Microsoft.VisualStudio.Web.CodeGeneration.Design/3.1.4

https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.4

https://www.nuget.org/packages/Npgsql.EntityFrameworkCore.PostgreSQL/3.1.4

# Si descargas el proyecto y no quieres instalar los paquetes
Ejecuta en la consola: dotnet restore Para que se te instalen automaticamente

# Despues de instalar paquetes (Vistas de Login, ForgotPassword, etc)
Ejecutar la siguiente instrucción: dotnet aspnet-codegenerator identity -dc La Carpeta donde esta alojado tu Aplicación Web .Data.ApplicationDbContext --files "Account.vista que quieren"

# Instalar herramienta (dotnet ef)
https://docs.microsoft.com/en-us/ef/core/cli/dotnet