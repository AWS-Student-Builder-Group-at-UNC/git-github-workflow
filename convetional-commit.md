# Conventional Commits

**Conventional Commits** es una convención de formato para escribir mensajes de commit en Git de forma clara, estandarizada y fácil de entender.

---

## Estructura

```text
<tipo>(<alcance opcional>): <descripción>
```

* **Tipo:** Obligatorio. Indica la intención del cambio (`feat`, `fix`, etc.).
* **Alcance (opcional):** El área o módulo del código afectado entre paréntesis (`auth`, `ui`, `api`).
* **Descripción:** Resumen breve del cambio en tiempo presente e imperativo (`agrega`, `corrige`, `elimina`).

---

## Tipos de Commit

| Tipo | Descripción | Ejemplo |
| :--- | :--- | :--- |
| **`feat`** | Añade una nueva funcionalidad. | `feat(auth): agrega inicio de sesión con Google` |
| **`fix`** | Arregla un error o bug en el código. | `fix(cart): corrige error al calcular el total` |
| **`docs`** | Cambios únicamente en la documentación. | `docs: actualiza instrucciones en el README` |
| **`style`** | Formato, espacios o comas sin alterar la lógica. | `style: aplica formato al archivo index.js` |
| **`refactor`** | Mejora el código sin añadir funciones ni arreglar bugs. | `refactor: simplifica consulta a la base de datos` |
| **`test`** | Añade o modifica pruebas (tests). | `test: agrega prueba para el registro de usuario` |
| **`chore`** | Tareas de mantenimiento o configuración del proyecto. | `chore: actualiza dependencias` |
| **`perf`** | Cambios de código que mejoran el rendimiento. | `perf: optimiza la carga de imágenes` |
| **`build`** | Modificaciones en el sistema de compilación o dependencias. | `build: configura webpack para producción` |
| **`ci`** | Cambios en integración continua (GitHub Actions, etc.). | `ci: agrega pipeline de despliegue` |

---

## Buenas Prácticas

1. **Usa minúsculas:** Inicia la descripción en minúscula (`feat: agrega...`).
2. **Tiempo presente:** Usa verbos en imperativo/presente (`agrega`, `corrige`, `elimina`).
3. **Sin punto final:** No coloques `.` al terminar la descripción.
4. **Commits atómicos:** Mantén cada commit enfocado en una sola tarea.

---

## Ejemplos Rápidos

- `feat: añade filtro por categoría de producto`
- `fix(login): resuelve bloqueo al ingresar clave incorrecta`
- `docs: añade diagrama de arquitectura del sistema`

