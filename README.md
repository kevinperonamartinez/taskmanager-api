# 📋 API de Gestión de Tareas

Una API RESTful desarrollada con **Kotlin + Spring Boot** que permite gestionar tareas (crear, leer, actualizar y eliminar). Diseñada con buenas prácticas, integración con base de datos PostgreSQL y preparada para ampliación con autenticación y Docker.

---

## 🚀 Tecnologías utilizadas

- ⚙️ Kotlin
- ☕ Spring Boot (Web, Data JPA)
- 🐘 PostgreSQL
- 🧪 Postman (para pruebas)
- 📦 Gradle
- 🐳 Docker (preparado para integrar)

---

## 📁 Estructura del proyecto

taskmanager/
├── controller/ # Controladores REST
├── model/ # Entidades JPA
├── repository/ # Interfaces de acceso a datos
├── service/ # Lógica de negocio
├── resources/
│ └── application.properties
└── build.gradle.kts


---

## ⚙️ Configuración

### 🛠️ Requisitos

- Java 17 o superior (compatible con Java 21)
- PostgreSQL
- Gradle
- Git

### 📦 Base de datos

1. Crear base de datos:

Nombre: taskmanagerdb
Usuario: taskuser
Contraseña: taskpass


2. Verifica el archivo de configuración:  
`src/main/resources/application.properties`

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/taskmanagerdb
spring.datasource.username=taskuser
spring.datasource.password=taskpass
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
server.port=8080

📦 Ejemplo JSON para crear una tarea
{
  "title": "Aprender Kotlin",
  "description": "Estudiar fundamentos y hacer prácticas"
}
