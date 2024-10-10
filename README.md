# Proyecto de Interacción con HTML y JavaScript

Este proyecto es un ejemplo de cómo interactuar con HTML y JavaScript para modificar contenido, atributos HTML y estilos CSS mediante código dinámico.

## Flujo de Trabajo con Git Flow

Git Flow es una metodología de trabajo para gestionar el desarrollo de software de manera organizada. Esta estrategia utiliza ramas específicas para diferentes etapas del ciclo de vida del proyecto.

### Ramas principales:

- `main`: Rama principal para la producción. Aquí se encuentra siempre el código listo para ser desplegado.
- `develop`: Rama para el desarrollo. Todo el trabajo de las nuevas funcionalidades se integra aquí antes de pasar a producción.

### Tipos de ramas en Git Flow:

1. **Feature branches (Ramas de características)**: Se usan para desarrollar nuevas funcionalidades. Se crean desde `develop` y se reintegran ahí una vez completadas.
   - Ejemplo:
     ```bash
     git flow feature start nombre-de-la-feature
     ```
2. **Release branches**: Se crean cuando se está preparando una nueva versión para producción. Esto permite realizar pruebas y correcciones antes de desplegar a `main`.
   - Ejemplo:
     ```bash
     git flow release start nombre-de-la-release
     ```
3. **Hotfix branches**: Se utilizan para corregir errores críticos directamente en producción. Se crean desde `main` y se reintegran tanto en `main` como en `develop`.
   - Ejemplo:
     ```bash
     git flow hotfix start nombre-del-hotfix
     ```

## Proceso seguido

1. **Inicialización de Git Flow**: El flujo de trabajo comenzó con la inicialización de Git Flow en el repositorio del proyecto.

   ```bash
   git flow init
