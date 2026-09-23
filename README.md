# TaskFlow

![GitHub last commit](https://img.shields.io/github/last-commit/usuario/taskflow)[cite: 5]
![GitHub issues](https://img.shields.io/github/issues/usuario/taskflow)[cite: 5]
![GitHub stars](https://img.shields.io/github/stars/usuario/taskflow)[cite: 5]

Aplicación para administrar tareas.[cite: 5]

## Tabla de contenidos
- [Descripción](#descripción)[cite: 5]
- [Funcionalidades](#funcionalidades)[cite: 5]
- [Tecnologías](#tecnologías)[cite: 5]
- [Instalación](#instalación)[cite: 5]
- [Uso](#uso)[cite: 5]
- [Contribuidores](#contribuidores)[cite: 5]

## Descripción
Aplicación sencilla para administrar tareas de un equipo.[cite: 5]

## Funcionalidades
- [x] Registrar tareas[cite: 5]
- [x] Editar tareas[cite: 5]
- [ ] Eliminar tareas[cite: 5]
- [ ] Asignar tareas a usuarios[cite: 5]

## Tecnologías
- Frontend
- API
- MySQL

## Requisitos
- Base de datos configurada.
- Entorno de ejecución de código.

## Instalación
1. Clonar el repositorio.[cite: 5]
2. Configurar la base de datos.[cite: 5]
3. Configurar las variables necesarias.[cite: 5]
4. Ejecutar la aplicación.[cite: 5]

## Capturas de pantalla
### Pantalla principal
![Pantalla principal](docs/img/inicio.png)[cite: 5]

### Gestión de tareas
![Gestión de tareas](docs/img/tareas.png)[cite: 5]

## Arquitectura
La aplicación está organizada en diferentes componentes que permiten gestionar
la interacción con el usuario, la autenticación, el acceso a datos y el registro
de actividades.[cite: 5]

```mermaid
flowchart LR
    U[Usuario] --> F[Frontend][cite: 5]
    F --> API[API][cite: 5]
    API --> AUTH[Autenticación][cite: 5]
    API --> DAO[DAO][cite: 5]
    DAO --> DB[(MySQL)][cite: 5]
    API --> LOG[Registro de actividad][cite: 5]
```