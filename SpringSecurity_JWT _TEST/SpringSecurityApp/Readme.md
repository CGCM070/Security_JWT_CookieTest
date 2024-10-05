
---

# Aplicación Spring Security JWT

## Introducción

Este proyecto es una aplicación Spring Boot que implementa autenticación y autorización basada en JWT (JSON Web Token). Incluye las siguientes características:

- **Registro y Login de Usuarios**: Los usuarios pueden registrarse e iniciar sesión. Al iniciar sesión, se genera un token JWT.
- **Control de Acceso Basado en Roles**: Diferentes niveles de acceso según los roles de usuario.
- **Validación de Tokens JWT**: Filtros personalizados para validar tokens JWT.
- **HSTS (HTTP Strict Transport Security)**: Configurado para forzar conexiones seguras (HTTPS).
- **CORS (Cross-Origin Resource Sharing)**: Configurado para permitir solicitudes de origen cruzado.

## Tecnologías Utilizadas

- Java
- Spring Boot
- Spring Security
- JWT
- Maven

## Estructura del Proyecto

- **Controller**: Maneja las solicitudes y respuestas HTTP.
- **Service**: Contiene la lógica de negocio para la autenticación y autorización de usuarios.
- **Filter**: Filtros personalizados para la validación de JWT.
- **Configuration**: Configuraciones de seguridad para la aplicación.



### Endpoints de la API

- **POST /auth-cookie/register**: Registrar un nuevo usuario.
- **POST /auth-cookie/login**: Iniciar sesión y recibir un token JWT.
- **GET /personas**: Acceder a un recurso protegido (requiere autenticación).

## Configuración de Seguridad

La configuración de seguridad se define en la clase `SecurityConfig`, que incluye ajustes para la validación de tokens JWT, control de acceso basado en roles y CORS.

---

