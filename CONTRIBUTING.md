# Directrices de Contribución

Este documento establece los estándares técnicos y procedimentales para contribuir a los repositorios de la organización **Linux y Open Source USM**. Se espera que todos los colaboradores sigan estas directrices para mantener la calidad, legibilidad y mantenibilidad del código.

## 1. Flujo de Trabajo (Workflow)

Utilizamos el modelo de colaboración **Fork & Pull**. No se permiten commits directos a la rama `main` o `master` bajo ninguna circunstancia.

1.  **Fork:** Realice un fork del repositorio objetivo a su cuenta personal.
2.  **Rama (Branch):** Cree una rama descriptiva para su trabajo.
    * Formato: `tipo/nombre-corto`
    * Ejemplo: `feat/autenticacion-oauth`, `fix/fuga-memoria-api`.
3.  **Desarrollo:** Implemente los cambios localmente.
4.  **Sincronización:** Asegúrese de que su rama esté actualizada con `upstream/main` antes de enviar cambios para evitar conflictos.
5.  **Pull Request:** Envíe un Pull Request (PR) hacia la rama principal del repositorio original.

## 2. Estándares de Código

Para garantizar la coherencia entre proyectos, se deben respetar las siguientes normas:

* **Clean Code:** El código debe ser autodocumentado, modular y respetar los principios SOLID donde aplique.
* **Comentarios:** El código debe estar comentado únicamente cuando la lógica de negocio sea compleja. Evite comentarios redundantes.
* **Archivos Ignorados:** Verifique que el archivo `.gitignore` esté configurado correctamente. No suba archivos de entorno local (`.env`, carpetas IDE, binarios compilados).
* **Linting:** Si el proyecto cuenta con herramientas de linter o formatters (Prettier, ESLint, Black, etc.), ejecútelos antes de realizar el commit.

## 3. Política de Commits

Adherimos a la especificación **Conventional Commits** para automatizar el versionado y la generación de changelogs.

La estructura del mensaje debe ser: `<tipo>: <descripción breve>`

**Tipos permitidos:**
* `feat`: Una nueva funcionalidad para el usuario.
* `fix`: Corrección de un error (bug).
* `refactor`: Cambio de código que no corrige errores ni añade funcionalidades (mejora de estructura/rendimiento).
* `docs`: Cambios exclusivamente en la documentación.
* `chore`: Tareas de mantenimiento, dependencias o configuración de build.

*Ejemplo correcto:* `feat: implementar endpoint de login con JWT`

## 4. Reporte de Incidentes (Issues)

Antes de abrir un issue, verifique que no exista uno similar abierto o cerrado.

* **Bug Reports:** Debe incluir pasos exactos de reproducción, entorno (SO, versión del lenguaje/framework) y logs de error si aplica.
* **Feature Requests:** Debe detallar la justificación técnica o funcional de la propuesta.

## 5. Proceso de Revisión (Code Review)

Todos los Pull Requests requieren la aprobación de al menos un mantenedor del proyecto.
* Sea receptivo a los comentarios durante la revisión de código.
* Si se solicitan cambios, realícelos en la misma rama y haga push; el PR se actualizará automáticamente.

---
**Nota:** Al participar en este proyecto, usted acepta cumplir con nuestro [Código de Conducta](CODE_OF_CONDUCT.md). El incumplimiento de estas normas puede resultar en la desestimación de sus contribuciones.
