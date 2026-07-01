# Introducción a GitHub — Demo práctica 🚀

Bienvenido/a. Este repositorio es un **espacio de práctica seguro** para hacer tu primer flujo completo en GitHub, el mismo que vimos en la presentación:

> **clone → editar → commit → push → Pull Request**

No puedes romper nada. La idea es que cada persona cree su propio documento y abra su primer Pull Request. ¡Manos a la obra!

---

## Lo que vas a hacer

1. **Clonar** este repositorio en tu ordenador.
2. **Crear una rama** (branch) con tu nombre.
3. **Crear un documento nuevo** dentro de la carpeta [`Crear_documento_aquí`](Crear_documento_aquí).
4. **Escribir algo** en él.
5. **Guardar los cambios** (commit).
6. **Subir la rama** (push).
7. **Abrir un Pull Request** (PR) para proponer tus cambios.

---

## Antes de empezar

Necesitas tener instalado:

- [Git](https://git-scm.com/downloads)
- [Visual Studio Code](https://code.visualstudio.com/)
- Una cuenta de GitHub con acceso a este repositorio

---

## Paso a paso

Puedes seguir los pasos con **comandos en la terminal** o usando la **interfaz gráfica de VSCode** (pestaña *Source Control*, el icono de las ramas a la izquierda). Abajo tienes las dos opciones.

### 1. Clonar el repositorio

Trae una copia del repositorio a tu ordenador.

```bash
git clone https://github.com/Simoneberhagen/Github-Demo.git
cd Github-Demo
```

> En VSCode: `Ctrl+Shift+P` → *Git: Clone* → pega la URL de arriba.

### 2. Crear tu rama

Trabajamos siempre en una rama propia, nunca directamente sobre `main`. Usa tu nombre para que sea fácil de identificar.

```bash
git checkout -b demo/tu-nombre
```

Por ejemplo: `git checkout -b demo/maria`

> En VSCode: haz clic en el nombre de la rama (abajo a la izquierda) → *Create new branch* → escribe `demo/tu-nombre`.

### 3. Crear tu documento

Dentro de la carpeta [`Crear_documento_aquí`](Crear_documento_aquí), crea un archivo nuevo con tu nombre, por ejemplo `maria.md`.

### 4. Escribir algo

Abre tu archivo y escribe lo que quieras: una presentación, tus notas de la sesión, o simplemente "¡Hola GitHub!". Guarda con `Ctrl+S`.

### 5. Preparar y guardar los cambios (commit)

Un *commit* es una foto de tus cambios con un mensaje que explica qué hiciste.

```bash
git add "Crear_documento_aquí/tu-nombre.md"
git commit -m "Añado mi documento de la demo"
```

> En VSCode: en *Source Control* verás tu archivo en *Changes*. Pulsa el `+` para prepararlo (*stage*), escribe un mensaje y pulsa *Commit*.

### 6. Subir tu rama (push)

Envía tu rama y tus commits a GitHub.

```bash
git push -u origin demo/tu-nombre
```

> En VSCode: pulsa *Publish Branch* / *Sync Changes*.

### 7. Abrir un Pull Request

1. Ve al repositorio en GitHub: <https://github.com/Simoneberhagen/Github-Demo>
2. Verás un aviso *"Compare & pull request"* → haz clic.
3. Comprueba que va de tu rama `demo/tu-nombre` hacia `main`.
4. Pon un título y una breve descripción.
5. Pulsa **Create pull request**.

¡Enhorabuena! 🎉 Acabas de completar el flujo completo de GitHub.

---

## Chuleta de comandos

```bash
git clone https://github.com/Simoneberhagen/Github-Demo.git   # copiar el repo
cd Github-Demo
git checkout -b demo/tu-nombre                                # crear tu rama
# ...crea y edita tu archivo en Crear_documento_aquí/...
git add "Crear_documento_aquí/tu-nombre.md"                   # preparar cambios
git commit -m "Añado mi documento de la demo"                 # guardar cambios
git push -u origin demo/tu-nombre                             # subir a GitHub
# ...abrir el Pull Request desde la web de GitHub...
```

---

## Glosario rápido

| Término | Qué significa |
|---|---|
| **Repositorio (repo)** | La carpeta del proyecto con todo su historial. |
| **Clonar** | Traer una copia del repo a tu ordenador. |
| **Rama (branch)** | Una línea de trabajo independiente para tus cambios. |
| **Commit** | Una foto guardada de tus cambios, con un mensaje. |
| **Push** | Subir tus commits a GitHub. |
| **Pull Request (PR)** | Una propuesta para incorporar tus cambios a `main`, revisable por el equipo. |
| **Merge** | Integrar los cambios del PR en `main`. |

---

¿Dudas? Pregunta durante la sesión — para eso está la demo. 🙌
