# 🏋️‍♂️ Sistema de Gestión de Gimnasio

Aplicación desarrollada en **.NET** siguiendo los principios de **Clean Architecture**, diseñada para administrar un gimnasio de manera eficiente.

---

## 📌 Descripción

Este sistema permite gestionar las operaciones principales de un gimnasio, incluyendo:

* Registro de socios
* Gestión de membresías
* Control de pagos
* Administración de Claes
* Seguimiento de asistencia

---

## 🧱 Arquitectura

El proyecto está estructurado siguiendo **Clean Architecture**, separando responsabilidades en distintas capas:

```
GymApp
│
├── ProyectoTIF.API             → Capa de presentación (Web API)
├── ProyectoTIF.Application     → Casos de uso
├── ProyectoTIF.Domain          → Entidades y lógica de negocio
└── ProyectoTIF.Infrastructure  → Acceso a datos y servicios externos
```

### 🔗 Dependencias

* API → Application
* Application → Domain
* Infrastructure → Application + Domain

---

## 🚀 Tecnologías utilizadas

* .NET 6/7/8
* ASP.NET Core Web API
* Entity Framework Core
* SQL Server (o cualquier DB relacional)
* Inyección de dependencias

---

## ⚙️ Instalación y ejecución

### 1. Clonar el repositorio

```
git clone https://github.com/WeFake123/ProyectoTIF.git
cd ProyectoTIF
```

### 2. Restaurar dependencias

```
dotnet restore
```

### 3. Ejecutar la aplicación

```
dotnet run --project ProyectoTIF.API
```

---

## 📊 Funcionalidades principales

### 👤 Socios

* Alta, baja y modificación de socios
* Consulta de información personal

### 💳 Membresías

* Creación de planes (mensual, anual, etc.)
* Asignación a socios

### 💰 Pagos

* Registro de pagos
* Control de vencimientos

### 📅 Asistencia

* Registro de ingreso al gimnasio
* Historial de asistencia

### 🏋️ Rutinas

* Creación y asignación de rutinas de entrenamiento

---

## 🧪 Testing (opcional)

Se pueden agregar pruebas unitarias para la capa Application:

```
dotnet test
```

---

## 📁 Estructura de carpetas sugerida

```
ProyectoTIF.Domain
 ├── Entities
 ├── Enums
 └── Interfaces

ProyectoTIF.Application
 ├── UseCases
 ├── DTOs
 └── Interfaces

ProyectoTIF.Infrastructure
 ├── Persistence
 └── Services

ProyectoTIF.API
 ├── Controllers
 └── Configurations
```

---

## 📌 Buenas prácticas implementadas

* Separación de responsabilidades
* Inversión de dependencias
* Código desacoplado
* Escalabilidad y mantenibilidad

---

## 📈 Mejoras futuras

* Autenticación con JWT
* Panel de administración (frontend)
* Notificaciones de vencimiento
* Integración con apps móviles

---

## 👨‍💻 Autor

Desarrollado como proyecto de aprendizaje en .NET y Clean Architecture.
