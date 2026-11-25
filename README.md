# Stork

**Several Claude Code agents working at once, without stepping on each other.**

Stork is a desktop app for macOS. Each task runs in its own _workspace_: a copy of your repo (a git
worktree) with its own branch, folder, ports and chats. Open five agents in parallel and the sidebar
shows which one is working, which is waiting for you and which has answered.

This repository only holds the downloads. The full documentation is at
**[sevenstork.com/apps/stork](https://sevenstork.com/apps/stork)** (English and Spanish).

_[Español abajo ↓](#espanol)_

---

## Download

[**Latest version for Mac**](https://github.com/FedericoSebastian/stork-releases/releases/latest/download/Stork-universal.dmg)
· macOS 11 or newer · Apple Silicon and Intel.

Open the `.dmg` and drag Stork to Applications. It's signed and notarized by Apple, so there's no
"unidentified developer" warning (the first launch still asks whether to open an app downloaded from
the internet; confirm with **Open**).

To update, download the new `.dmg` and drop it over the old one. Your projects, chats and accounts
live separately in `~/.stork` and aren't touched. Older versions stay forever on the
[releases page](https://github.com/FedericoSebastian/stork-releases/releases).

## What you need

- **git** and **claude** ([Claude Code](https://claude.com/claude-code)) installed. Stork checks for them at startup and tells you what's missing.
- **gh** (GitHub CLI) is optional: without it there are no PRs, issues or CI, but everything else works.
- A Claude account (subscription or API). A local model works too.

## Getting started in 4 steps

1. **Open Stork.** While you have no projects it walks you through it: it checks the tools, gets you
   logged in to Claude and offers to create your first project.
2. **Create a project** with one or more repos (a local folder, a GitHub repo or a new one). A
   project can hold several repos, and each workspace makes a worktree of every one.
3. **New workspace.** That's a task: its own branch, its own folder and its own 10 ports. Ask the
   agent for something in the chat; on your first message the branch renames itself after what you asked.
4. **Review and ship.** In the right-hand panel you read the diff, comment on lines, commit, create
   the PR and follow CI without leaving the app.

## What you can do

| | Guide |
| --- | --- |
| Several agents at once, each on its own branch and folder | [Projects and workspaces](https://sevenstork.com/apps/stork/en/proyectos) |
| Approve or reject what the agent wants to do, undo the last turn, use skills and commands | [The chat](https://sevenstork.com/apps/stork/en/chat) |
| Diff with per-line comments, commits, PRs, CI and merge | [Review and publish changes](https://sevenstork.com/apps/stork/en/cambios) |
| Run each workspace's app on its own ports, with its variables and scripts | [Variables, scripts and services](https://sevenstork.com/apps/stork/en/servicios) |
| Private variables kept in the keychain that Claude never receives | [Variables, scripts and services](https://sevenstork.com/apps/stork/en/servicios#environment-variables) |
| Several Claude and GitHub accounts, with their limits and usage in view | [Profiles and accounts](https://sevenstork.com/apps/stork/en/cuentas) |
| Alerts when an agent needs you, in the Dock and the menu bar | [Notifications, limits and usage](https://sevenstork.com/apps/stork/en/avisos) |
| Buttons with your own prompts for repeated tasks | [Actions and skills](https://sevenstork.com/apps/stork/en/acciones) |
| Keyboard shortcuts | [Shortcuts and search](https://sevenstork.com/apps/stork/en/atajos) |

## If something goes wrong

There's a [Common problems](https://sevenstork.com/apps/stork/en/problemas) page: what to do when
Stork can't find `claude`, when a branch is busy in another folder, when a port is taken or when an
agent is left waiting.

---

<a id="espanol"></a>

# Stork (Español)

**Varios agentes de Claude Code trabajando a la vez, sin pisarse.**

Stork es una app de escritorio para macOS. Cada tarea corre en su propio _workspace_: una copia de tu
repo (un git worktree) con su rama, su carpeta, sus puertos y sus chats. Abrís cinco agentes en
paralelo y desde la barra lateral ves cuál trabaja, cuál te espera y cuál ya respondió.

Este repositorio es sólo para las descargas. La documentación completa está en
**[sevenstork.com/apps/stork](https://sevenstork.com/apps/stork)** (español e inglés).

## Descargar

[**Última versión para Mac**](https://github.com/FedericoSebastian/stork-releases/releases/latest/download/Stork-universal.dmg)
· macOS 11 o más nuevo · Apple Silicon e Intel.

Abrí el `.dmg` y arrastrá Stork a Aplicaciones. Está firmada y notarizada por Apple: abre sin avisos
de "app no identificada" (la primera vez macOS igual te pregunta si querés abrir una app bajada de
internet; confirmá con **Abrir**).

Para actualizar, bajás el `.dmg` nuevo y lo arrastrás encima del anterior. Tus proyectos, chats y
cuentas viven aparte, en `~/.stork`, y no se tocan. Las versiones anteriores quedan para siempre en
la [lista de releases](https://github.com/FedericoSebastian/stork-releases/releases).

## Qué necesitás

- **git** y **claude** ([Claude Code](https://claude.com/claude-code)) instalados. Stork los busca al abrir y te dice cuál falta.
- **gh** (GitHub CLI) es opcional: sin él no hay PRs, issues ni CI, pero todo lo demás funciona.
- Una cuenta de Claude (suscripción o API). También podés usar un modelo local.

## Empezar en 4 pasos

1. **Abrí Stork.** Mientras no tengas proyectos te guía: verifica las herramientas, te hace iniciar
   sesión en Claude y te ofrece crear el primer proyecto.
2. **Creá un proyecto** con uno o varios repos (una carpeta local, un repo de GitHub o uno nuevo).
   Un proyecto puede tener varios repos y cada workspace arma un worktree de cada uno.
3. **Nuevo workspace.** Es una tarea: rama propia, carpeta propia y 10 puertos propios. Pedile algo
   al agente en el chat; cuando mandes el primer mensaje, la rama se renombra sola según lo que
   pediste.
4. **Revisá y publicá.** En el panel de la derecha mirás el diff, comentás líneas, commiteás, creás
   el PR y seguís el CI sin salir de la app.

## Lo que podés hacer

| | Guía |
| --- | --- |
| Varios agentes a la vez, cada uno en su rama y su carpeta | [Proyectos y workspaces](https://sevenstork.com/apps/stork/es/proyectos) |
| Aprobar o rechazar lo que el agente quiere hacer, deshacer el último turno, usar skills y comandos | [El chat](https://sevenstork.com/apps/stork/es/chat) |
| Diff con comentarios por línea, commits, PRs, CI y merge | [Revisar y publicar cambios](https://sevenstork.com/apps/stork/es/cambios) |
| Levantar la app de cada workspace en sus propios puertos, con sus variables y scripts | [Variables, scripts y servicios](https://sevenstork.com/apps/stork/es/servicios) |
| Variables privadas que van al llavero y que Claude nunca recibe | [Variables, scripts y servicios](https://sevenstork.com/apps/stork/es/servicios#variables-de-entorno) |
| Varias cuentas de Claude y de GitHub, con sus límites y su uso a la vista | [Perfiles y cuentas](https://sevenstork.com/apps/stork/es/cuentas) |
| Avisos cuando un agente te necesita, en el Dock y en la barra de menú | [Avisos, límites y uso](https://sevenstork.com/apps/stork/es/avisos) |
| Botones con tus propios prompts para tareas repetidas | [Acciones y skills](https://sevenstork.com/apps/stork/es/acciones) |
| Atajos de teclado | [Atajos y búsqueda](https://sevenstork.com/apps/stork/es/atajos) |

## Si algo falla

Está la página de [Problemas comunes](https://sevenstork.com/apps/stork/es/problemas): qué hacer si
Stork no encuentra `claude`, si una rama está ocupada por otra carpeta, si un puerto quedó tomado o
si un agente se queda esperando.
