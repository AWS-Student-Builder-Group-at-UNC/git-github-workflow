# ✅ Solución guiada — Lección 01

Esta práctica no tiene una única respuesta "correcta" porque es de exploración. Acá te cuento qué deberías haber notado en cada paso, para que confirmes que estás mirando lo importante.

## 1. Cantidad de commits

En un repositorio grande y activo como VS Code, vas a encontrar **decenas de miles de commits** acumulados a lo largo de varios años. Esto es exactamente el punto: Git escala sin problema desde un proyecto de una sola persona hasta uno con cientos de colaboradores y años de historia, sin perder ni un solo cambio registrado.

## 2. El mensaje del commit elegido

Si elegiste un commit al azar, probablemente encontraste dos tipos de mensajes:

- Mensajes **claros**, tipo `"Fix crash when closing editor with unsaved changes"` — se entiende exactamente qué se solucionó sin mirar el código.
- Mensajes **poco claros**, tipo `"fix"` o `"updates"` — no dicen nada útil.

Esto no es casualidad: es la diferencia entre un buen hábito de commits y uno malo, algo que vamos a trabajar explícitamente en la **Lección 11**. Ya desde ahora, empezá a notar qué mensajes te resultan útiles cuando los leés como alguien externo al proyecto.

## 3. El diff (líneas verdes y rojas)

Lo importante acá no es que entiendas el código en sí, sino que confirmes esta idea: **Git no te obliga a adivinar qué cambió** — te lo muestra explícitamente, línea por línea, con colores. Esa es la base de cómo funciona la revisión de código en un equipo (lo vas a ver en detalle en la Lección 07, Pull Requests).

## 4. Ramas activas

Un proyecto grande como VS Code tiene múltiples ramas activas al mismo tiempo — gente trabajando en distintas funcionalidades en paralelo, sin pisarse entre sí. Esto es exactamente el problema que resuelven las ramas, y es el tema completo de las **Lecciones 03 y 07**.

---

### 🔑 La idea que te tenés que llevar de esta lección

No necesitás memorizar nada todavía. Solo quedate con esto: **todo lo que acabás de ver (commits, mensajes, diffs, ramas) es información que Git genera automáticamente**, sin que nadie tenga que escribir a mano un changelog o nombrar archivos como `version_final_v2.docx`. En la próxima lección vas a crear tu propio commit por primera vez, desde el navegador, y vas a ver este mismo tipo de historial pero en un repo tuyo.
