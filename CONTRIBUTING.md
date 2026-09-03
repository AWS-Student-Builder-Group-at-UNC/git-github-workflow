# Cómo contribuir

Este repositorio forma parte de la biblioteca de aprendizaje del **AWS Student Builder Group UNC**.

## 📌 Antes de contribuir
- Cada lección debe mantener la estructura estándar: `README.md`, `practica.md` y `solucion.md`.
- No se debe agregar más de 1 práctica por lección (siguiendo el criterio pedagógico del área).
- El TP integrador se ubica únicamente en la carpeta `21-integrador`.
- Antes de redactar o actualizar una lección, revisá la sección **Desglose de Contenidos por Lección** para asegurarte de abarcar todos los temas planificados.

## ✍️ Estilo de contenido
- Explicá siempre el **por qué**, no solo el **cómo**.
- Todo el código y comandos deben estar explicados en español, desglosando líneas o parámetros nuevos.
- Enfocá los ejemplos en casos de uso reales de trabajo en equipo (entornos de desarrollo, CI/CD, infraestructura).

## 🔄 Proceso de contribución

Si es tu primera vez contribuyendo en GitHub o abriendo un Pull Request, seguí este paso a paso:

1. **Hacé un Fork**: Presioná el botón **Fork** (arriba a la derecha en la página de GitHub de este repo) para crear una copia en tu cuenta.
2. **Cloná tu fork y creá una rama (Remplaza TU-USUARIO y feat_leccion_x_ejemlo)**:

```bash
git clone [https://github.com/TU-USUARIO/git-github-workflow.git](https://github.com/TU-USUARIO/git-github-workflow.git)
cd git-github-workflow
git switch -c feat_leccion_x_ejemlo
```


3. **Hacé tus cambios y commitealos**:
```bash
git add .
git commit -m "docs: redactar leccion 05 commit en profundidad"

```


4. **Subí la rama a tu fork(Remplaza feat/leccion-x-ejemlo)**:
```bash
git push -u origin feat/leccion-x-ejemlo

```


5. **Abrí el Pull Request (PR)**: Entrá a tu fork en GitHub, hacé clic en el botón **Compare & pull request** y enviá la propuesta hacia la rama `main` del repositorio original con una descripción clara de lo aportado.

---

## 📋 Desglose de Contenidos por Lección

Quien contribuya redactando o mejorando el contenido de una lección debe asegurarse de abarcar los siguientes puntos mínimos por tema:

### 🟢 Nivel Fundamentos

#### 01 — ¿Qué es Git y por qué existe?

* Problema que resuelve el control de versiones (versionado manual de archivos, caos de nombres).
* Qué es un **commit** (snapshot, no un archivo suelto).
* Git vs. GitHub (herramienta local vs. plataforma en la nube).
* Alternativas a GitHub (mención breve: GitLab, Bitbucket).

#### 02 — Tu primer repositorio

* Crear un repositorio desde GitHub (sin terminal todavía).
* Qué es el `README.md` y por qué GitHub lo renderiza automáticamente.
* Editar un archivo desde la web y qué es un commit ahí (autor, mensaje, timestamp).
* Ver el historial de commits en la UI.

#### 03 — Ramas y Pull Requests

* Qué es una rama (concepto: línea de trabajo paralela).
* Crear una rama desde GitHub.
* Qué es un Pull Request (PR) y para qué sirve.
* Revisar diffs dentro de un PR (UI).
* Mergear un PR desde GitHub.
* Mecanismo interno del merge: fast-forward vs. merge commit, con los comandos clave para visualizarlo (`git merge`, `git log --graph`).

#### 04 — Instalando y configurando Git

* Instalación en Windows (Git Bash / winget), Linux (`apt`), macOS (`brew`).
* Verificar instalación (`git --version`).
* Configuración inicial: `git config --global user.name`, `user.email`.
* Qué es el editor por defecto de Git (y cómo cambiarlo, ej. a VS Code).
* Autenticación con GitHub desde terminal (mención de HTTPS + token vs. SSH — profundidad real en Lección 06).

#### 05 — El commit en profundidad

* **Staging area**: qué es, por qué existe un paso intermedio entre "modificar" y "commitear".
* Configuración extra del sistema operativo para ver extensiones de archivo y archivos ocultos (muy útil para desarrollo).
* `git init` para crear un repo local.
* `git add` (archivo completo) vs. `git add -p` (por partes/hunks).
* `git status` (leer bien la salida: unstaged / staged / untracked).
* `git diff` (working directory vs. staging) vs. `git diff --staged` (staging vs. último commit).
* `git commit` vs. `git commit --amend` (corregir el último commit sin crear uno nuevo).
* `git log` — variantes útiles: `--oneline`, `--graph`, `-p`.
* Anatomía de un commit: hash, autor, committer, mensaje, padre(s).

#### 06 — Conectando con GitHub (remotos)

* Qué es un "remoto" (`origin`).
* `git clone` (traer un repo completo con su historial).
* `git remote -v`, `git remote add`.
* `git push` (con especial atención a `push -u` la primera vez, y qué hace el `-u`).
* `git pull` = `fetch` + `merge` (explicar que no es un comando atómico "mágico").
* `git fetch` solo (traer cambios sin mezclarlos, para qué sirve tenerlos separados).
* Autenticación real: token personal (HTTPS) vs. llave SSH — con criterio de cuándo usar cada una.

#### 07 — Ramas por comandos

* `git branch` (listar, crear).
* `git switch` (moderno) vs. `git checkout` (histórico — mencionar que van a ver ambos "en la vida real").
* `git merge` — qué es un **fast-forward merge** vs. un **merge commit** (mecánica interna, no solo el resultado).
* Ramas de tracking: `git branch -vv`, cómo se relaciona una rama local con su remota.
* Borrar ramas: `git branch -d` vs. `-D` (por qué Git te protege con `-d` y qué hace `-D`).

#### 08 — Fork vs. Clone

* Clonar un repo propio vs. hacer fork de un repo ajeno.
* Qué pasa "atrás de escena" cuando hacés fork (copia completa a tu cuenta).
* Cómo mantener tu fork actualizado con el original (`upstream`, `git remote add upstream`, `git fetch upstream`).
* Cuándo usar cada estrategia (proyecto propio vs. contribuir a uno ajeno).

#### 09 — Deshacer cambios

* `git restore` (descartar cambios en working directory).
* `git restore --staged` (sacar del staging sin perder el cambio).
* `git reset` — variantes: `--soft`, `--mixed` (default), `--hard` (y el riesgo real de cada una).
* `git revert` (deshacer con un commit nuevo, seguro en ramas compartidas) vs. `reset` (reescribe historia, peligroso si ya se compartió).
* Criterio: cuándo usar `reset` (local, no compartido) vs. `revert` (ya pusheado / compartido con otros).

#### 10 — Conflictos de merge

* Cómo se relaciona esta lección con lo visto en "Ramas por comandos" y "Deshacer cambios" al momento de resolver un conflicto.
* Por qué ocurre un conflicto (dos ramas tocaron la misma línea).
* Anatomía de las marcas de conflicto en un archivo (`<<<<<<<`, `=======`, `>>>>>>>`).
* Resolución manual paso a paso.
* Herramientas visuales de resolución (VS Code merge editor, o la UI de GitHub para conflictos simples).
* Criterio: cuándo comunicarse con el equipo en vez de resolver "a ciegas".

---

### 🟡 Nivel Intermedio

#### 11 — `.gitignore` y buenas prácticas de commits

* Qué versionar y qué no (secretos, `node_modules`, archivos generados, `.env`).
* Sintaxis de `.gitignore` (patrones, wildcards, negación con `!`).
* Qué hacer si ya versionaste algo por error (`git rm --cached`).
* Conventional Commits (formato `tipo(scope): mensaje`, tipos comunes: `feat`/`fix`/`docs`/`chore`/`refactor`).
* Por qué importa un buen mensaje de commit (legibilidad del historial, changelogs automáticos).

#### 12 — Flujos de trabajo

* Git Flow (ramas `develop`, `feature/*`, `release/*`, `hotfix/*`) — cuándo tiene sentido (releases programados, versionado formal).
* GitHub Flow (simplificado: `main` + ramas de feature + PR) — cuándo tiene sentido (deploy continuo).
* Trunk-Based Development (commits chicos y frecuentes directo a `main` o ramas de vida muy corta) — contexto de CI/CD maduro y feature flags.
* Criterio de elección según tamaño de equipo y frecuencia de release.

#### 13 — Stash: guardando cambios sin commitear

* Punto de partida del nivel intermedio: Git va más allá de ramas, commits, push y pull.
* `git stash` (guardar cambios sin commitear, para cambiar de contexto rápido).
* `git stash list`, `git stash pop` vs. `git stash apply` (diferencia: pop borra el stash, apply no).
* `git stash push -m "mensaje"` (nombrar el stash para no perderse con varios).
* Caso de uso real: "tengo que hacer un fix urgente en otra rama pero no quiero commitear esto a medio hacer".

#### 14 — Tags y versionado semántico

* `git tag` (crear, listar, tags anotados vs. ligeros).
* Versionado semántico (SemVer): `MAJOR.MINOR.PATCH`, qué significa cada número.
* Relación entre tags y Releases de GitHub.
* `git push --tags` (por qué los tags no se pushean automáticamente con `git push`).

---

### 🔴 Nivel Avanzado

#### 15 — Cherry-pick

* `git cherry-pick <hash>` (traer un commit puntual de otra rama).
* Caso de uso real: hotfix que necesita aplicarse en `main` y en una rama de release simultáneamente.
* Conflictos durante un cherry-pick (mismo mecanismo que un merge, pero acotado a un commit).

#### 16 — Rebase interactivo

* `git rebase -i` (reescribir historial local antes de compartirlo).
* Comandos dentro del editor interactivo: `pick`, `squash`/`fixup`, `reword`, `drop`, `reorder`.
* Diferencia entre rebase y merge (reescribe vs. preserva historia).
* **Regla de oro**: nunca rebasear una rama que ya compartiste/pusheaste con otros.
* Conflictos durante un rebase (se resuelven "commit por commit", distinto flujo que en un merge).

#### 17 — Reflog

* `git reflog` (historial interno de movimientos de `HEAD`, distinto de `git log`).
* Recuperar un commit "perdido" después de un `reset --hard` o un rebase mal hecho.
* Por qué casi nunca perdés trabajo realmente en Git (ventana de garbage collection).

#### 18 — Git bisect

* `git bisect start`, `bisect good`, `bisect bad` (búsqueda binaria sobre el historial).
* Caso de uso real: "esto funcionaba hace 2 semanas, ¿en qué commit se rompió?".
* `git bisect run <script>` (automatizar la búsqueda con un test).

#### 19 — Git hooks

* Qué es un hook (script que Git ejecuta en momentos clave del flujo).
* Hooks locales comunes: `pre-commit`, `commit-msg`, `pre-push`.
* Qué es un **linter** (herramienta que valida estilo/errores de código antes de aceptarlo) — explicar desde cero.
* Caso de uso real: bloquear un commit si el mensaje no sigue Conventional Commits, o si el código no pasa el linter.
* Mención de herramientas que facilitan esto (Husky, pre-commit framework).

#### 20 — CI/CD

* Qué es **CI/CD** y qué problema busca resolver en el desarrollo de software.
* Qué significa **Continuous Integration (CI)** y para qué sirve.
* Qué significa **Continuous Delivery (CD)** y para qué sirve.
* Diferencia entre **Continuous Delivery** y **Continuous Deployment**.
* Qué es un **pipeline** y cuáles son sus etapas principales.
* Flujo básico de un pipeline: `git push → build → tests → linter → deploy`.
* Qué sucede cuando una etapa del pipeline falla.
* Caso de uso real: ejecutar automáticamente tests y validaciones en cada `push` o Pull Request.
* Relación entre CI/CD, Git y los repositorios de código.
* Ejemplo de herramientas de CI/CD: **GitHub Actions**, GitLab CI/CD y Jenkins (mención breve).

#### 21 — TP Integrador

* Combina: fork, rama, PR, conflicto de merge, rebase interactivo, resolución con criterio y CI/CD.
* Simulación de un flujo de colaboración real de punta a punta.
* Estructura: `tp-integrador.md` + carpeta `solucion/`.
