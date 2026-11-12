# Evolución de la Programación — Documental Interactivo

Página web estilo documental sobre la historia de los lenguajes de programación, con resúmenes claros de cada era.

Inspirada en el concepto de [calcsolver.pro](https://calcsolver.pro/): una interfaz principal “educativa” y un acceso **oculto** a una sección de juegos que **no se guarda en el historial del navegador**.

## Cómo usarlo

1. Abre `index.html` en el navegador (o actívalo con GitHub Pages).
2. Lee el documental sobre Fortran, COBOL, LISP, BASIC, C, C++, Java, Python, JavaScript, Go, Rust, etc.
3. **Acceso oculto a juegos**: en la esquina inferior derecha del encabezado hay un pequeño círculo casi invisible. Haz clic en él.
4. Se abre el **Arcade Oculto** (Snake, Memoria, Click Rush, Pong Lite).
5. Al salir, vuelves al documental. El historial del navegador **solo contiene la página principal** (no se añade ninguna entrada al historial al abrir o cerrar los juegos).

## Características técnicas

- 100 % frontend (HTML + CSS + JavaScript vanilla).
- Sin frameworks.
- Sin cambios de URL ni `history.pushState` al abrir juegos → solo se registra la página principal.
- Juegos implementados nativamente (canvas + DOM).
- Responsive y con diseño oscuro moderno.

## Activar GitHub Pages

1. Ve a **Settings → Pages** del repositorio.
2. Source: Deploy from a branch → `main` / root.
3. En unos minutos tendrás la web en:
   `https://romanprogramador-stack.github.io/programacion-evolucion/`

## Estructura

```
programacion-evolucion/
├── index.html   # Toda la aplicación (documental + juegos)
└── README.md
```

Hecho para aprender y divertirse.
