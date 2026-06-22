# Matemática Discreta · Laboratorio Interactivo

Colección de simuladores, juegos y quizzes interactivos del curso de **Matemática Discreta**, organizados **por tema** (no por semana). Todo el sitio es estático: funciona en GitHub Pages sin servidor, sin compilación y sin conexión a internet.

**Docente:** Dr. José Herrera Quispe

---

## Contenido por tema

| # | Tema | Actividad | Archivo | Formato |
|---|------|-----------|---------|---------|
| 01 | Lógica y demostración | Lógica proposicional (suite completa) | `logica_proposicional.html` | Interactivo |
| 01 | Lógica y demostración | Álgebra de Boole y circuitos | `algebra_boole_lab.html` | Laboratorio |
| 01 | Lógica y demostración | Quiz de lógica | `logica_quiz.html` | Quiz |
| 02 | Conjuntos, relaciones y funciones | Quiz de conjuntos | `conjuntos_quiz.html` | Quiz |
| 03 | Conteo y combinatoria | Conteo Master | `conteo_combinatoria.html` | Juego |
| 04 | Sistemas de numeración | Numeración y color | `sistemas_numeracion.html` | Visualizador |
| 05 | Grafos | Grafos: simulador | `grafos_simulador.html` | Simulador |
| 05 | Grafos | Pac-Grafo | `grafos_pacgrafo.html` | Arcade |
| 05 | Grafos | Quiz de grafos | `grafos_quiz.html` | Quiz |
| 06 | Árboles, expresiones y pilas | Árboles: simulador | `arboles_simulador.html` | Simulador |
| 06 | Árboles, expresiones y pilas | Expresiones: simulador | `expresiones_simulador.html` | Simulador |
| 07 | Autómatas y lenguajes | Autómatas finitos y gramáticas | `automatas_simulador.html` | Simulador |
| 08 | Criptografía y teoría de números | Cifrados: RSA, César y Afín | `criptografia_rsa.html` | Interactivo |

**13 actividades · 8 temas · 5 formatos** (Simulador, Juego/Arcade, Quiz, Laboratorio/Visualizador, Interactivo).

---

## Estructura del repositorio

```
.
├── index.html                  ← página principal (hub)
├── README.md
├── vendor/                     ← REQUERIDO (React + lucide locales)
│   ├── react.min.js
│   ├── react-dom.min.js
│   └── lucide-react.min.js
├── logica_proposicional.html
├── algebra_boole_lab.html
├── logica_quiz.html
├── conjuntos_quiz.html
├── conteo_combinatoria.html
├── sistemas_numeracion.html
├── grafos_simulador.html
├── grafos_pacgrafo.html
├── grafos_quiz.html
├── arboles_simulador.html
├── expresiones_simulador.html
├── automatas_simulador.html
└── criptografia_rsa.html
```

> **Importante:** la carpeta `vendor/` es obligatoria. Las actividades `logica_proposicional.html` y `criptografia_rsa.html` (originalmente componentes React) cargan React y lucide **desde esa carpeta local**, por lo que funcionan sin conexión y sin paso de compilación. Si no subes `vendor/`, esas dos actividades quedarán en blanco.

---

## Publicar en GitHub Pages

1. Crea un repositorio (ej. `matematica-discreta`) y sube **todos** los archivos, incluyendo la carpeta `vendor/`.
2. En **Settings → Pages**, en *Source* elige la rama `main` y la carpeta `/root`.
3. En ~1 minuto el sitio queda publicado en `https://<usuario>.github.io/<repo>/`.

---

## Agregar más recursos

El índice está organizado por tema. Para sumar una actividad nueva:

1. Sube su archivo `.html` con un nombre por contenido (ej. `relaciones_funciones.html`).
2. En `index.html`, copia una tarjeta `<a class="act live" ...>` dentro de la sección del tema y ajusta título, descripción, *badge* y enlace.
3. Si la actividad es un componente React, reutiliza la carpeta `vendor/` ya incluida.

> En la sección **Conjuntos, relaciones y funciones** hay una tarjeta *Próximamente* lista para reemplazar cuando esté el recurso de relaciones y funciones.

---

## Identidad visual

Paleta unificada en torno al **índigo `#5B49F0`** sobre fondo claro, con tipografías Space Grotesk (títulos), Inter (texto) y JetBrains Mono (código).

Tres actividades conservan **a propósito** su paleta temática porque el color forma parte del aprendizaje: Pac-Grafo (estética arcade), el laboratorio de Álgebra de Boole (terminal verde) y el visualizador de numeración (RGB). El hub y los quizzes mantienen la identidad índigo común.
