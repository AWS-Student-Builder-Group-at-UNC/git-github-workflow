<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="AWS" width="90"/>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git" width="60"/>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" width="60"/>
</div>

<h1 align="center">Git & GitHub Workflow</h1>
<p align="center"><i>AWS Student Group UNC — Aprendizaje Práctico</i></p>

---

> Control de versiones y flujo de trabajo colaborativo: la base de cualquier proyecto de software o infraestructura.

## 📌 ¿Qué vas a aprender acá?

Git es la herramienta que usa prácticamente toda la industria para versionar código e infraestructura (sí, también Terraform, Kubernetes manifests, y pipelines de CI/CD). No es opcional: es el piso mínimo para trabajar en cualquier equipo técnico. Acá vas a aprender desde cero — primero **viendo cómo funciona visualmente en GitHub**, y después replicando exactamente lo mismo desde la terminal, para que entiendas qué hace cada comando en vez de memorizarlo a ciegas.

## 🧭 Nivel

🟢 **Principiante** — no necesitás experiencia previa con control de versiones.

## 💻 Sobre tu sistema operativo

Este repo funciona igual en **Windows, Linux y macOS**. Vas a encontrar los pasos de instalación para cada sistema por separado, pero a partir de ahí **los comandos de Git son idénticos** sin importar dónde los ejecutes — la terminal cambia, Git no.

## ✅ Prerrequisitos generales

- Cuenta de GitHub creada ([github.com](https://github.com) — es gratis).
- Ganas de romper cosas sin miedo — para eso está la Lección 08 😉

## 🗺️ Índice de lecciones

| # | Lección | Nivel | Descripción corta |
|---|---------|-------|--------------------|
| 01 | [¿Qué es Git y por qué existe?](./01-que-es-git/README.md) | 🟢 | El problema que resuelve el control de versiones|
| 02 | [Tu primer repo](./02-primer-repo-web/README.md) | 🟢 | Crear un repo, editar archivos y hacer tu primer commit desde GitHub |
| 03 | [Colaborar: ramas y Pull Requests](./03-ramas-pr-web/README.md) | 🟢 | Crear una rama, proponer un cambio y fusionalo|
| 04 | [Instalando y configurando Git](./04-instalacion-git/README.md) | 🟢 | Windows, Linux y macOS — mismos comandos, distinta instalación |
| 05 | [Lo mismo que ya sabés hacer, ahora por comandos](./05-primer-repo-terminal/README.md) | 🟢 | `init`, `add`, `commit`, `status`, `log` |
| 06 | [Conectar tu compu con GitHub](./06-conectar-remoto/README.md) | 🟢 | `clone`, `remote`, `push`, `pull`, `fetch` |
| 07 | [Ramas por comandos](./07-ramas-terminal/README.md) | 🟢 | `branch`, `switch`, `merge` — lo que ya hiciste en la Lección 03, ahora en terminal |
| 08 | [Deshacer cambios sin miedo](./08-deshacer-cambios/README.md) | 🟢 | `diff`, `restore`, `reset`, `revert` — viajar en el tiempo con criterio |
| 09 | [Fork vs. Clone](./09-fork-vs-clone/README.md) | 🟡 | Cómo colaborar en proyectos que no son tuyos |
| 10 | [Conflictos de merge y rebase básico](./10-merge-conflictos/README.md) | 🟡 | Resolver conflictos con criterio, no a los golpes |
| 11 | [.gitignore y buenas prácticas de commits](./11-buenas-practicas/README.md) | 🟡 | Qué versionar, qué no, y cómo escribir mensajes útiles |
| 12 | [Flujos de trabajo](./12-flujos-de-trabajo/README.md) | 🟡 | Qué estrategia usa la industria y cuándo conviene cada una |
| 13 | [TP Integrador](./13-integrador/README.md) | 🟡 | Simulación de colaboración real: fork, rama, PR, conflicto y merge |

## 🚦 Cómo usar este repo (paso a paso, desde cero)

**1. Cloná el repo a tu máquina** (si solo vas a practicar localmente):
```bash
git clone https://github.com/AWS-Student-Builder-Group-at-UNC/git-github-workflow.git
cd git-github-workflow
```

**2. O hacé fork** (si vas a subir tus propias soluciones a tu cuenta de GitHub — recomendado):
- Click en "Fork" arriba a la derecha de este repo en GitHub.
- Esto crea una copia completa en **tu** cuenta.
- Después clonás **tu fork**, no el original:
```bash
git clone https://github.com/TU-USUARIO/git-github-workflow.git
```
> 💡 No te preocupes si "clonar" y "hacer fork" todavía no te cierran del todo — es exactamente el tema de la Lección 09, y para las primeras lecciones (01 a 03) ni siquiera vas a necesitar clonar nada: se hacen enteras desde el navegador.

**3. Recorré las lecciones en orden.** Cada una asume lo aprendido en la anterior — especialmente las lecciones 05 a 08, que son la versión "por comandos" de lo que ya hiciste visualmente en las lecciones 02 y 03.

**4. En cada lección:** leé el `README.md` → resolvé `practica.md` **antes** de mirar `solucion.md`.

**5. Al terminar la Lección 12**, encarás `13-integrador/` — ahí vas a simular un flujo de colaboración real de punta a punta, combinando web y terminal.

## 🧭 Buenas prácticas y criterio de la vida real

Más allá de los comandos, en cada lección vas a encontrar contexto sobre **cómo se usa esto en un equipo de verdad**:

- Por qué nunca se pushea directo a `main` en un proyecto real (y qué son los rulesets/branch protection).
- Cómo escribir un mensaje de commit que tu compañero de equipo entienda sin preguntarte nada.
- Cuándo conviene `rebase` y cuándo es una mala idea (spoiler: nunca en ramas compartidas).
- Qué hacer cuando rompiste algo y tenés pánico — Git casi siempre tiene forma de volver atrás.
- Cómo se ve una buena Pull Request vs. una que nadie quiere revisar.

Este repo no busca enseñarte comandos exóticos — busca que salgas con el criterio mínimo para trabajar en un equipo sin generar caos.

## 🧹 Sobre costos y recursos

Este repo no requiere cuenta de AWS ni genera costos — todo el contenido es local o dentro de GitHub (gratuito).

## 🤝 Contribuciones

¿Encontraste un error o querés proponer una lección nueva? Mirá [`CONTRIBUTING.md`](./CONTRIBUTING.md).

## 📄 Licencia

Este contenido se distribuye bajo licencia [MIT](./LICENSE).

---
<p align="center"><i>Parte de la biblioteca de Aprendizaje Práctico — AWS Student Group UNC</i></p>
