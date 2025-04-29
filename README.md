# TodoApi - API REST con ASP.NET Core y SQLite

Esta API REST fue desarrollada utilizando ASP.NET Core 8.0 y SQLite como base de datos. Proporciona endpoints para gestionar una lista de tareas (TODO list) con persistencia de datos.

## 🚀 Características

- CRUD completo para tareas (TodoItems)
- Persistencia de datos con SQLite
- Documentación con Swagger/OpenAPI
- Arquitectura RESTful
- Protección contra sobre-exposición de datos mediante DTOs

## 📋 Requisitos Previos

- [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0)
- [Visual Studio Code](https://code.visualstudio.com/) o [Visual Studio 2022](https://visualstudio.microsoft.com/vs/)

## 🛠️ Instalación

1. Clona el repositorio:

```bash
git clone <tu-repositorio>
cd TodoApi
```

2. Restaura los paquetes NuGet:

```bash
dotnet restore
```

3. Aplica las migraciones de la base de datos:

```bash
dotnet ef database update
```

## 🚀 Ejecución

1. Ejecuta el proyecto:

```bash
dotnet run
```

2. Abre tu navegador y ve a:

```
http://localhost:5155/swagger/index.html
```

## 📌 Endpoints API

| Método | Ruta                | Descripción                   |
| ------ | ------------------- | ----------------------------- |
| GET    | /api/todoitems      | Obtiene todas las tareas      |
| GET    | /api/todoitems/{id} | Obtiene una tarea por ID      |
| POST   | /api/todoitems      | Crea una nueva tarea          |
| PUT    | /api/todoitems/{id} | Actualiza una tarea existente |
| DELETE | /api/todoitems/{id} | Elimina una tarea             |

## 🗄️ Estructura de la Base de Datos

La base de datos SQLite (`todo.db`) contiene la siguiente tabla:

### TodoItems

- Id (INTEGER, Primary Key)
- Name (TEXT)
- IsComplete (INTEGER/BOOLEAN)
- Secret (TEXT)

## 🔧 Tecnologías Utilizadas

- ASP.NET Core 8.0
- Entity Framework Core
- SQLite
- Swagger/OpenAPI

## 📦 Paquetes NuGet Principales

- Microsoft.EntityFrameworkCore.Sqlite
- SQLitePCLRaw.bundle_e_sqlite3
- Swashbuckle.AspNetCore

## 🤝 Contribuir

1. Haz un Fork del proyecto
2. Crea tu rama de características (`git checkout -b feature/AmazingFeature`)
3. Haz commit de tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Haz Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia MIT - mira el archivo [LICENSE.md](LICENSE.md) para detalles

## ✨ Autor

Tu nombre - [@tutwitter](https://twitter.com/tutwitter)

---

⌨️ con ❤️ por [Tu Nombre](https://github.com/tusername)
