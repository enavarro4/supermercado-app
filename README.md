# Supermercado API

API REST para gestionar la operativa basica de un supermercado.

## Overview

Este proyecto esta construido con Spring Boot y orientado a exponer endpoints HTTP para un backend de supermercado.

Estado actual del repositorio:
- Aplicacion base de Spring Boot inicializada.
- Configuracion de seguridad presente, con todas las rutas permitidas por ahora.
- Dependencias de JPA, Web MVC y H2 incluidas para avanzar rapidamente en desarrollo.

## Stack tecnico

- Java 17
- Spring Boot 4.0.5
- Spring Web MVC
- Spring Data JPA
- Spring Security
- H2 Database (runtime)
- Maven Wrapper (`mvnw`, `mvnw.cmd`)

## Estructura principal

- `src/main/java/com/supermercado/app/AppApplication.java`: punto de entrada de la app.
- `src/main/java/com/supermercado/app/config/SecurityConfig.java`: seguridad HTTP actual.
- `src/main/resources/application.properties`: configuracion base.

## Ejecucion local

En Windows (PowerShell):

```powershell
mvn spring-boot:run
```

En MAC/Linux:

```bash
mvn spring-boot:run
```

La API quedara disponible en:
- `http://localhost:8080`

## Tests

```powershell
.\mvnw.cmd test
```

## Roadmap sugerido

- Definir entidades principales (`Producto`, `Carrito`).
- Crear capas `controller`, `service` y `repository`.
- Implementar CRUD de productos y categorias.
- Agregar validaciones y manejo global de errores.

