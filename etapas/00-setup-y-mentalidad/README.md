# Etapa 0 · Setup y mentalidad

⏱️ **Duración:** ~1 semana · **Dedicación:** ~10h · 🔴 Sin empezar

> Antes de escribir una línea de app, montás tu taller y aprendés la herramienta que vas a usar TODOS los días: git. Esta etapa parece "poca cosa" y es la que separa a quien programa de quien improvisa.

## Por qué esta etapa existe

Vos ya tenés teoría. El problema es el puente a la práctica. Y la práctica real tiene un requisito invisible que los tutoriales ignoran: **el entorno y el control de versiones**. Sin git, cada experimento que rompés es irrecuperable. Con git, podés romper con confianza. Por eso git NO va al final del plan — va acá, en la sesión 2, y lo usás en cada entrega de acá en adelante.

## Objetivos medibles

Al terminar esta etapa, tenés que poder demostrar cada uno de estos:

- [ ] **Entorno funcionando:** VS Code + Node LTS + terminal + gestor de paquetes; corrés `node --version` y `npm --version` sin errores.
- [ ] **Modelo mental de la web:** explicás con tus palabras qué pasa desde que escribís una URL hasta que ves la página (DNS → request HTTP → servidor → response → render).
- [ ] **Repo `learning-journal` creado:** con al menos 5 commits atómicos de mensajes claros.
- [ ] **Flujo de PR completo:** creaste una branch, hiciste cambios, abriste un Pull Request en GitHub y lo mergeaste.
- [ ] **Quiz aprobado** con ≥80%.

## Teoría mínima (20/80)

### 1. Cómo funciona la web (el 20% que explica el 80%)

- **Cliente** = tu navegador. **Servidor** = una computadora que responde. Se hablan por **HTTP**.
- Escribís una URL → el navegador resuelve el dominio a una IP vía **DNS** → manda una **request HTTP** → el servidor devuelve una **response** (HTML, JSON, etc.) → el navegador **renderiza**.
- Métodos HTTP que importan: **GET** (traer), **POST** (crear), **PUT/PATCH** (modificar), **DELETE** (borrar).
- Códigos de estado: **2xx** ok, **3xx** redirección, **4xx** error del cliente (404 = no existe, 401/403 = permisos), **5xx** error del servidor.

### 2. El entorno de trabajo

- **Node.js**: runtime de JavaScript fuera del navegador. Instalá la versión **LTS**.
- **Gestor de paquetes**: `npm` (viene con Node) o `pnpm` (más rápido, recomendado). Instala librerías y corre scripts.
- **VS Code**: tu editor. Extensiones mínimas: ESLint, Prettier, y la de tu terminal integrada.
- **Terminal**: aprendé lo esencial — `cd`, `ls`/`dir`, `mkdir`, `pwd`. No le tengas miedo.

### 3. Git — el 20% que usás el 80% del tiempo

```bash
git init                      # inicializar repo
git status                    # ver qué cambió
git add <archivo>             # preparar cambios (staging)
git add .                     # preparar todo
git commit -m "mensaje"       # guardar un snapshot
git log --oneline             # ver historial
git branch <nombre>           # crear branch
git switch <nombre>           # cambiar de branch
git switch -c <nombre>        # crear y cambiar
git merge <nombre>            # fusionar una branch
git push                      # subir a GitHub
git pull                      # traer cambios de GitHub
git clone <url>               # copiar un repo remoto
```

**Commit atómico** = un commit hace UNA cosa y su mensaje la describe. Malo: `"cambios"`. Bueno: `"add login form validation"`. Los mensajes van en **inglés**, en imperativo, estilo *conventional commits* (`feat:`, `fix:`, `docs:`, `chore:`).

**Flujo básico (el que vas a repetir siempre):**
1. `git switch -c feature/algo` (nueva branch)
2. Trabajás, hacés commits atómicos
3. `git push -u origin feature/algo`
4. Abrís un **Pull Request** en GitHub
5. Se mergea a `main`

## Recursos 20/80

- [MDN — Cómo funciona la web](https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/How_the_Web_works)
- [Git — documentación oficial (Pro Git, gratis)](https://git-scm.com/book/es/v2) — leé solo capítulos 1-3.
- [GitHub Docs — Hello World](https://docs.github.com/es/get-started/quickstart/hello-world)
- [Node.js — descarga LTS](https://nodejs.org/)

> No leas los libros enteros. Leé lo justo para hacer los entregables de `sesiones.md`. Volvés a la doc cuando la necesites.

## Siguiente paso

Abrí [sesiones.md](sesiones.md) y empezá por la Sesión 1.
