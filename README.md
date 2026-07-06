<div align="center">
  <!-- Aquí puedes colocar un banner minimalista o un logo. Sugerencia: una imagen en escala de grises o alto contraste -->
  <img src="./docs/assets/logo.png" alt="Logo del Sistema" width="20%">

  # ◾ Sistema de Gestión Académica ◾

  *Una arquitectura moderna para la administración integral de perfiles, materias y evaluaciones.*

  <br />

  <!-- Badges monocromáticos para un look más limpio y profesional -->
  [![FastAPI](https://img.shields.io/badge/API-FastAPI-111111?style=flat-square&logo=fastapi&logoColor=white)](#)
  [![React & Vite](https://img.shields.io/badge/Web-React_Vite-111111?style=flat-square&logo=react&logoColor=white)](#)
  [![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-111111?style=flat-square&logo=postgresql&logoColor=white)](#)
  [![Docker](https://img.shields.io/badge/Infrastructure-Docker-111111?style=flat-square&logo=docker&logoColor=white)](#)

</div>

<br />

> **Propósito:** Este proyecto proporciona una plataforma centralizada y escalable para gestionar el ecosistema académico, separando claramente la lógica de negocio, la interfaz de usuario y la persistencia de datos mediante contenedores.

---

## ⚆ Arquitectura del Sistema

El proyecto está diseñado bajo una arquitectura de microservicios contenerizados, dividida en tres módulos principales:

*   **`web` (Frontend):** Interfaz de usuario reactiva y minimalista construida con React y empaquetada con Vite para un rendimiento óptimo.
*   **`api` (Backend):** Núcleo lógico del sistema desarrollado en FastAPI, encargado de la validación, seguridad y procesamiento de las reglas de negocio.
*   **`db` (Base de Datos):** Motor relacional en PostgreSQL que asegura la integridad de la información académica.

## ⚆ Estructura de Datos y Modelado

El modelo relacional está diseñado para soportar la complejidad de una institución educativa real, implementando **Control de Acceso Basado en Roles (RBAC)**. 

### Características Principales del Modelo:
1.  **Perfiles Modulares:** Separación de la entidad principal de autenticación de los perfiles específicos de `Estudiantes` y `Profesores` (Relaciones 1:1).
2.  **Flexibilidad de Roles:** Un usuario puede poseer múltiples responsabilidades dentro del sistema (ej. Docente y Coordinador Administrativo) gracias a la tabla puente de roles.
3.  **Gestión Académica:** Trazabilidad completa desde la inscripción del usuario en materias, hasta el registro detallado de sus evaluaciones y calificaciones.

> 🔗 **Explora el modelo de datos detallado:** Puedes revisar el [Diagrama Entidad-Relación y el esquema DBML](./docs/database/architecture.md) en nuestra documentación técnica.

---

<div align="center">
  <i>Proyecto en construcción.</i>
</div>