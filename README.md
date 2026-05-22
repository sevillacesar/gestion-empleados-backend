<div align="center">
  <h1>Gestión de Empleados - Backend</h1>
  <p><strong>API REST para gestión de empleados con Spring Boot y PostgreSQL</strong></p>

  <p>
    <img src="https://img.shields.io/badge/Java-17-ED8B00?style=flat-square&logo=java" alt="Java 17"/>
    <img src="https://img.shields.io/badge/Spring_Boot-2.7.15-6DB33F?style=flat-square&logo=spring-boot" alt="Spring Boot 2.7.15"/>
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql" alt="PostgreSQL"/>
    <img src="https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apache-maven" alt="Maven"/>
    <img src="https://img.shields.io/badge/Lombok-FF0000?style=flat-square&logo=lombok" alt="Lombok"/>
  </p>
</div>

---

## Descripción

API RESTful para la gestión de empleados construida con Spring Boot, JPA/Hibernate y PostgreSQL. Proporciona operaciones CRUD completas con validación de datos y manejo de errores.

## Stack

| Tecnología | Versión |
|------------|---------|
| Java | 17 |
| Spring Boot | 2.7.15 |
| Spring Data JPA | 2.7.15 |
| PostgreSQL | 15.x |
| Maven | 3.x |
| Lombok | 1.18.x |

## Requisitos

- Java 17+
- Maven 3.x
- PostgreSQL 15+

## Instalación y ejecución

### 1. Clonar

```bash
git clone https://github.com/sevillacesar/gestion-empleados-backend.git
cd gestion-empleados-backend
```

### 2. Configurar base de datos

Crea una base de datos PostgreSQL:

```sql
CREATE DATABASE gestion_empleados;
```

Configura las credenciales en `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/gestion_empleados
spring.datasource.username=tu_usuario
spring.datasource.password=tu_password
spring.jpa.hibernate.ddl-auto=update
```

### 3. Compilar y ejecutar

```bash
mvn clean install
mvn spring-boot:run
```

### 4. Probar la API

```bash
curl http://localhost:8080/api/empleados
```

## API Endpoints

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| `GET` | `/api/empleados` | Listar todos los empleados |
| `GET` | `/api/empleados/{id}` | Obtener empleado por ID |
| `POST` | `/api/empleados` | Crear nuevo empleado |
| `PUT` | `/api/empleados/{id}` | Actualizar empleado |
| `DELETE` | `/api/empleados/{id}` | Eliminar empleado |

## Licencia

Distribuido bajo MIT License.
