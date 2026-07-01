# Guion de la demo — Introducción a GitHub 🎬

Guion para la persona que presenta. Lo que está en **negrita** = lo que puedes *decir*. El texto normal = lo que *haces*. Dura unos **15–20 min**.

> Antes de empezar: abre VSCode, la web del repo (<https://github.com/Simoneberhagen/Github-Demo>) y la terminal. Cierra el correo y las notificaciones.

---

## 0. Inicio (1 min)

> **"Ya hemos visto la teoría. Ahora lo hacemos de verdad, juntos. Vais a ver todo el proceso de GitHub, y luego lo hacéis vosotros. No se puede romper nada, tranquilos."**

> **"El proceso es siempre igual. Son cinco pasos: clonar, editar, guardar, subir y abrir un Pull Request. Vamos uno a uno."**

---

## 1. Clonar el repositorio (2 min)

Acción: abre la terminal en una carpeta vacía.

> **"Primero traemos una copia del proyecto a nuestro ordenador. Esto se llama *clonar*."**

```bash
git clone https://github.com/Simoneberhagen/Github-Demo.git
cd Github-Demo
```

> **"Ya tengo todo el proyecto en mi ordenador. Mirad: aparece la carpeta, y dentro está el README con los pasos."**

Abre la carpeta en VSCode: `code .` o *File → Open Folder*.

---

## 2. Crear una rama (2 min)

> **"Nunca trabajamos sobre `main`. `main` es la versión buena, la que ve todo el mundo. Creamos una *rama*: un espacio propio para hacer cambios sin molestar a nadie."**

```bash
git checkout -b demo/simon
```

> **"Le pongo mi nombre para reconocerla fácil. Ahora trabajo en `demo/simon`, no en `main`."**

Señala el nombre de la rama abajo a la izquierda en VSCode.

> **"¿Veis esto de aquí abajo? VSCode me dice siempre en qué rama estoy. Mirad esto siempre: es importante saber dónde estáis."**

---

## 3. Crear y editar un documento (3 min)

> **"Vamos a hacer un cambio real. Dentro de la carpeta `Crear_documento_aquí` voy a crear mi documento."**

Acción: crea un archivo nuevo en `Crear_documento_aquí/`, por ejemplo `simon.md`. Escribe algo que se vea.

> **"Escribo lo que sea... por ejemplo: '¡Hola GitHub! Este es mi primer cambio.' Y guardo con Control+S."**

Abre la pestaña *Source Control* (el icono de las ramas, a la izquierda).

> **"En cuanto guardo, mirad el panel de la izquierda: GitHub ve que hay un archivo nuevo. Todavía no está guardado en el historial, solo lo ha detectado."**

---

## 4. Guardar los cambios — commit (3 min)

> **"Ahora hago un *commit*. Un commit es como una foto de mis cambios, con una nota que dice qué hice. Es un punto al que siempre puedo volver."**

Con el ratón (mejor para la demo):
- Pulsa el `+` al lado del archivo para prepararlo.
- Escribe la nota: `Añado mi documento de la demo`.
- Pulsa **Commit**.

> **"Escribo una nota clara que diga qué cambié. Una buena nota ayuda a todo el equipo a entender el historial. Y pulso Commit."**

(Lo mismo en la terminal, por si alguien pregunta:)

```bash
git add "Crear_documento_aquí/simon.md"
git commit -m "Añado mi documento de la demo"
```

---

## 5. Subir a GitHub — push (2 min)

> **"Hasta ahora esto solo está en mi ordenador. Con el *push* lo subo a GitHub, a la nube, para que los demás lo puedan ver."**

Pulsa **Publish Branch** / **Sync Changes** en VSCode.

```bash
git push -u origin demo/simon
```

Refresca la web del repo.

> **"Si voy a GitHub y refresco... ahí está mi rama. Ya está en la nube."**

---

## 6. Pull Request (3 min)

> **"El último paso: pedir que mi cambio entre en `main`. Esto se hace con un *Pull Request*, o PR. Es una petición para juntar mi trabajo con el resto, y deja que otra persona lo revise antes."**

En la web:
1. GitHub muestra el botón **"Compare & pull request"** → haz clic.
2. Mira que vaya de `demo/simon` → hacia `main`.
3. Pon un título y una nota corta.
4. **Create pull request**.

> **"Aquí cualquiera del equipo puede comentar, sugerir cambios y, cuando esté bien, aprobarlo. Por esto es seguro trabajar en equipo: nada entra en `main` sin pasar por aquí."**

(Si quieres cerrar el proceso:)

> **"Y cuando el PR está aprobado, se hace *merge*, y mi cambio ya está dentro de `main`. Fin del proceso."**

---

## 7. Ahora vosotros

> **"Ahora os toca a vosotros. Tenéis todos los pasos en el README del repositorio. Es fácil: cada uno crea su documento en la carpeta `Crear_documento_aquí` y abre su primer Pull Request."**

Dile al público:
- **"Abrid el README del repo. Ahí está todo escrito."**
- **"Paso 1: clonad el repositorio."**
- **"Paso 2: cread vuestra rama con vuestro nombre — `demo/vuestro-nombre`."**
- **"Paso 3: cread un archivo con vuestro nombre en la carpeta y escribid algo."**
- **"Paso 4: commit, push, y abrid el Pull Request."**
- **"Yo voy pasando por si alguien se atasca. Sin prisa, y no se puede romper nada."**

---

## Final

> **"Esto que acabáis de hacer es lo mismo que usan los equipos de programación cada día. Quedaos con una idea: rama, commit, push, Pull Request. Ese es el proceso."**

> **"Preguntas, cuando queráis."**

---

## 🆘 Ayuda rápida (si alguien se atasca)

| Problema | Qué hacer |
|---|---|
| "¿En qué rama estoy?" | `git branch` (la del `*`), o mira abajo a la izquierda en VSCode. |
| "Se me ha olvidado crear la rama" | `git checkout -b demo/tu-nombre` (se lleva los cambios sin guardar). |
| "No me deja subir (push)" | Mira que hiciste commit antes: `git status`. |
| "No veo el botón de Pull Request" | Refresca la web del repo, o ve a *Pull requests → New*. |
| "He editado en `main` sin querer" | Haz `git checkout -b demo/tu-nombre` ahora y guarda ahí. |
| "Sale un error raro" | Sin problema, es una demo. Borra la carpeta y vuelve a clonar. |



DELETE THIS