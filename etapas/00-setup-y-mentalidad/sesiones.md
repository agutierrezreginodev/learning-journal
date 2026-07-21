# Etapa 0 · Plan de sesiones

> ~4 sesiones de 2.5h. Cada sesión sigue el ritmo: repaso activo (15') → concepto (45') → práctica (60') → cierre + commit (20').

---

## Sesión 1 · El entorno y cómo funciona la web

**Concepto (45'):** Leé la sección "Cómo funciona la web" y "El entorno de trabajo" del [README](README.md). Instalá Node LTS, VS Code y un gestor de paquetes.

**Práctica (60'):**
- Verificá con `node --version`, `npm --version`.
- Creá una carpeta, abrila en VS Code, y desde la terminal integrada creá un archivo `hola.js` con `console.log("Hola mundo")` y corrélo con `node hola.js`.
- Escribí en un archivo de texto, con tus palabras, qué pasa cuando escribís `google.com` y apretás Enter.

**🎯 Entregable:** Archivo `notas/como-funciona-la-web.md` con tu explicación del ciclo request/response + captura de `node hola.js` funcionando.

---

## Sesión 2 · Git desde cero

**Repaso activo (15'):** Explicá en voz alta el ciclo request/response de la sesión anterior.

**Concepto (45'):** Leé la sección "Git — el 20%" del README y los capítulos 1-2 de Pro Git.

**Práctica (60'):**
- `git init` en una carpeta nueva.
- Creá archivos, hacé `git add` y `git commit` con mensajes claros (mínimo 3 commits).
- Practicá `git status` y `git log --oneline` después de cada paso.
- Rompé algo a propósito y volvé a un commit anterior para sentir el poder del versionado.

**🎯 Entregable:** Un repo local con mínimo 3 commits atómicos y mensajes en inglés estilo conventional commits.

---

## Sesión 3 · GitHub y el flujo de Pull Request

**Repaso activo (15'):** Rehacé de memoria los comandos git de la sesión anterior.

**Concepto (45'):** Leé GitHub Hello World. Entendé qué es un remoto (`origin`), una branch y un Pull Request.

**Práctica (60'):**
- Creá una cuenta de GitHub (si no tenés) y un repo nuevo llamado `learning-journal`.
- Conectá tu repo local al remoto y hacé `git push`.
- Creá una branch `feature/primer-cambio`, hacé un cambio, pusheala y abrí un **Pull Request**.
- Mergealo a `main`.

**🎯 Entregable:** El repo `learning-journal` en GitHub con al menos 1 PR mergeado. Pegá el link del PR en tus notas.

---

## Sesión 4 · Montar el learning-journal + mentalidad

**Repaso activo (15'):** Explicá qué es una branch y para qué sirve un PR.

**Concepto (45'):** Releé la sección "Filosofía" del [README raíz](../../README.md). Este repo `learning-journal` va a ser tu bitácora de TODO el plan.

**Práctica (60'):**
- Estructurá el `learning-journal` con carpetas por etapa: `etapa-00/`, `etapa-01/`, etc.
- Creá un `README.md` que explique qué es este repo.
- Anotá tus primeras entradas: qué aprendiste esta semana y qué dudas te quedaron.

**🎯 Entregable:** `learning-journal` estructurado y commiteado, listo para acompañarte todo el plan.

---

## Cierre de etapa

1. Completá el [quiz.md](quiz.md) y verificá que sacaste ≥80%.
2. Cerrá el [mini-proyecto.md](mini-proyecto.md).
3. Marcá los objetivos cumplidos en el [ROADMAP](../../ROADMAP.md) y cambiá el estado de la etapa a 🟢.
