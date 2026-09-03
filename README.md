<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="AWS" width="90"/>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git" width="60"/>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" width="60"/>
</div>

<h1 align="center">Git & GitHub Workflow</h1>
<p align="center"><i>AWS Student Builder Group UNC — Aprendizaje Práctico</i></p>

---

> Control de versiones y flujo de trabajo colaborativo: la base de cualquier proyecto de software o infraestructura.

## 📌 ¿Qué vas a aprender acá?

Git es la herramienta que usa prácticamente toda la industria para versionar código e infraestructura (sí, también Terraform, Kubernetes manifests, y pipelines de CI/CD). No es opcional: es el piso mínimo para trabajar en cualquier equipo técnico. Acá vas a aprender desde los conceptos más básicos hasta temas que le interesan a quien ya usa Git y quiere manejarlo con criterio real de equipo: rebase, resolución de conflictos, CI/CD y más.

## 🧭 Niveles

🟢 Fundamentos &nbsp;|&nbsp; 🟡 Intermedio &nbsp;|&nbsp; 🔴 Avanzado

## ✅ Prerrequisitos generales

- Cuenta de GitHub creada ([github.com](https://github.com), es gratis).
- Ganas de romper cosas sin miedo, para eso está la Lección 09 😉

## 🗺️ Índice de lecciones

| # | Lección | Nivel | Descripción corta |
|---|---------|-------|--------------------|
| 01 | [¿Qué es Git y por qué existe?](./01-que-es-git/README.md) | 🟢 | El problema que resuelve el control de versiones |
| 02 | [Tu primer repositorio](./02-primer-repositorio/README.md) | 🟢 | Crear un repo, editar archivos y tu primer commit desde GitHub |
| 03 | [Ramas y Pull Requests](./03-ramas-pull-requests/README.md) | 🟢 | Crear una rama, proponer un cambio, fusionarlo y entender qué pasó por detrás |
| 04 | [Instalando y configurando Git](./04-instalacion-git/README.md) | 🟢 | Windows, Linux y macOS, mismos comandos, distinta instalación |
| 05 | [El commit en profundidad](./05-commit-en-profundidad/README.md) | 🟢 | Staging area, `add`, `status`, `diff`, `commit --amend`, `log` |
| 06 | [Conectando con GitHub](./06-conectando-remoto/README.md) | 🟢 | Remotos: `clone`, `remote`, `push`, `pull`, `fetch` |
| 07 | [Ramas por comandos](./07-ramas-comandos/README.md) | 🟢 | `branch`, `switch`, `merge`, ramas de tracking |
| 08 | [Fork vs. Clone](./08-fork-vs-clone/README.md) | 🟢 | Cómo colaborar en proyectos que no son tuyos |
| 09 | [Deshacer cambios](./09-deshacer-cambios/README.md) | 🟢 | `restore`, `reset`, `revert`, viajar en el tiempo con criterio |
| 10 | [Conflictos de merge](./10-conflictos-de-merge/README.md) | 🟢 | Resolverlos con criterio, no a los golpes |
| 11 | [.gitignore y buenas prácticas de commits](./11-buenas-practicas/README.md) | 🟡 | Qué versionar, qué no, y Conventional Commits |
| 12 | [Flujos de trabajo](./12-flujos-de-trabajo/README.md) | 🟡 | Git Flow, GitHub Flow, Trunk-Based, cuándo conviene cada uno |
| 13 | [Stash](./13-stash/README.md) | 🟡 | Guardar cambios sin commitear para cambiar de contexto rápido |
| 14 | [Tags y versionado semántico](./14-tags-versionado/README.md) | 🟡 | Tags, SemVer y Releases de GitHub |
| 15 | [Cherry-pick](./15-cherry-pick/README.md) | 🔴 | Traer un commit puntual de otra rama |
| 16 | [Rebase interactivo](./16-rebase-interactivo/README.md) | 🔴 | Reescribir historial local con criterio |
| 17 | [Reflog](./17-reflog/README.md) | 🔴 | Recuperar lo que parecía perdido |
| 18 | [Git bisect](./18-git-bisect/README.md) | 🔴 | Encontrar automáticamente el commit que rompió algo |
| 19 | [Git hooks](./19-git-hooks/README.md) | 🔴 | Automatizar validaciones antes de commit/push |
| 20 | [CI/CD](./20-ci-cd/README.md) | 🔴 | Qué es un pipeline y cómo se conecta con Git |
| 21 | [TP Integrador](./21-integrador/README.md) | 🔴 | Fork, rama, PR, conflicto, rebase y CI/CD, todo junto |

## 🚦 Cómo usar este repo (paso a paso, desde cero)

**1. Cloná el repo a tu máquina** (si solo vas a practicar localmente):
```bash
git clone https://github.com/AWS-Student-Builder-Group-at-UNC/git-github-workflow.git
cd git-github-workflow
```

**2. O hacé fork** (si vas a subir tus propias soluciones a tu cuenta de GitHub, recomendado):
- Click en "Fork" arriba a la derecha de este repo en GitHub.
- Esto crea una copia completa en **tu** cuenta.
- Después clonás **tu fork**, no el original:
```bash
git clone https://github.com/TU-USUARIO/git-github-workflow.git
```
> 💡 No te preocupes si "clonar" y "hacer fork" todavía no te cierran del todo: es exactamente el tema de la Lección 08, y para las primeras lecciones (01 a 03) ni siquiera vas a necesitar clonar nada, se hacen enteras desde el navegador.

**3. Recorré las lecciones en orden.** Cada una asume lo aprendido en la anterior.

**4. En cada lección:** leé el `README.md`, resolvé `practica.md` **antes** de mirar `solucion.md`.

**5. Al terminar la Lección 20 (CI/CD)**, encarás `21-integrador/`: ahí vas a simular un flujo de colaboración real de punta a punta, combinando todo lo visto en el repo.

## 🧭 Buenas prácticas y criterio de la vida real

Más allá de los comandos, en cada lección vas a encontrar contexto sobre **cómo se usa esto en un equipo de verdad**:

- Por qué nunca se pushea directo a `main` en un proyecto real (y qué son los rulesets/branch protection).
- Cómo escribir un mensaje
