# Etapa 0 · Quiz de autoevaluación

> Respondé sin mirar. Después compará con las respuestas al final. Necesitás **≥80%** (10/12) para avanzar. Si no llegás, repasá y volvé a intentar.

## Preguntas

1. ¿Qué diferencia hay entre un cliente y un servidor en la web?
R/ El cliente es la aplicación, puede ser web, movil, o hasta una API, que realiza una petición HTTP al servidor para obtener una respuesta o enviar información. El servidor es quien revisa las solicitudes, las procesa y en caso tal sea necesario, envia una respuesta al cliente de acuerdo a la logica por detrás de la API.
2. Ordená lo que pasa cuando escribís una URL: render, request HTTP, resolución DNS, response del servidor.
R/ DNS, Request, Response, Render
3. ¿Qué método HTTP usás para *traer* datos y cuál para *crear* datos?
R/ Para traer, GET. Para crear, POST
4. ¿Qué significa un código de estado 404? ¿Y un 500? ¿Y un 401?
R/ 404: No encontro la redirección del sitio. 500: Error en el servidor. 401: Error de autenticación
5. ¿Qué es Node.js y en qué se diferencia de correr JavaScript en el navegador?
R/ Node.js es el entorno de ejecución de javascript, es parecido a la JVM. Nos permite correr codigo JavaScript en nuestra terminal, como si lo hicieramos en el navegador.
6. ¿Para qué sirve un gestor de paquetes como npm o pnpm?
R/ Para instalar y gestionar librerias y paquetes para el lenguaje de programación que estemos usando.
7. ¿Qué hace `git add` y en qué se diferencia de `git commit`?
R/ git add nos sirve para añadir cambios realizados en un archivo o tenerlos en cuenta en el commit que vamos a realizar. git commit nos sirve para guardar los cambios realizados y luego subirlos al repositorio
8. ¿Qué es un commit atómico y por qué importa?
R/ Un commit atómico es aquel en el que solo se modifica o se realiza una task, es importante para la trazabilidad de las modificaciones que los commits no sean tan extensos al momento de revisarlos.
9. ¿Qué comando crea una nueva branch y te cambia a ella en un solo paso?
R/ git branch <name>. git switch <name>
10. ¿Qué es un Pull Request y para qué se usa?
R/ Sirve para solicitar al administrador del repositorio, unir los cambios que realizamos con una de las ramas del repositorio.
11. ¿Qué diferencia hay entre `git push` y `git pull`?
R/ git push es para subir cambios al repo, y git pull, para traer los ultimos cambios de una rama.
12. ¿Por qué conviene trabajar en branches en vez de commitear siempre en `main`?
R/ Para mejorar el trabajo colaborativo, y no estropear accidentalmente el codigo en producción que por lo general se encuentra en main. Es mejor crear nuevas ramas para las modificaciones y luego crear los PR para su validación previa.

---

## Respuestas

1. El **cliente** (navegador) pide recursos; el **servidor** los provee/responde. Se comunican por HTTP.
2. Resolución DNS → request HTTP → response del servidor → render.
3. **GET** para traer, **POST** para crear.
4. **404** = recurso no encontrado (error del cliente). **500** = error interno del servidor. **401** = no autenticado (falta identidad).
5. Node.js es un **runtime** que ejecuta JavaScript fuera del navegador (en tu máquina/servidor). En el navegador, JS tiene acceso al DOM; en Node tiene acceso al sistema de archivos, red, etc.
6. Para instalar/gestionar dependencias (librerías) y correr scripts del proyecto.
7. `git add` **prepara** cambios en el staging area; `git commit` los **guarda** como un snapshot en el historial.
8. Un commit que hace **una sola cosa** con un mensaje que la describe. Importa porque hace el historial legible y permite revertir cambios puntuales.
9. `git switch -c <nombre>` (o el clásico `git checkout -b <nombre>`).
10. Una solicitud para **fusionar** los cambios de una branch en otra; permite revisión antes de mergear.
11. `push` **sube** tus commits al remoto; `pull` **trae** los commits del remoto a tu repo local.
12. Porque aislás el trabajo en progreso, no rompés `main` (la rama estable), y permitís revisión vía PR antes de integrar.

---

**Puntaje:** 11 / 12 (92%) → ✅ ≥80%, avanzá. Repasar: pregunta 9 (comando de un solo paso: git switch -c / git checkout -b).
