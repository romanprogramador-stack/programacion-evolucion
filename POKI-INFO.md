# Sobre Poki y juegos embebidos

## Por qué Poki no se puede "ejecutar dentro" de otra web

Poki.com (y CrazyGames, etc.) envían cabeceras HTTP como:

- `X-Frame-Options: DENY` o `SAMEORIGIN`
- Content-Security-Policy con `frame-ancestors 'none'`

Eso **impide** que su página se muestre dentro de un `<iframe>` en otro dominio. No es un fallo de nuestro código: lo bloquean ellos a propósito.

## Qué sí funciona en CodeTimeline

1. **Juegos nativos** (Snake, Pong, Memoria, Click Rush) → 100% dentro de la página.
2. **Algunos juegos** que permiten embed (2048, Hextris, Dino, etc.).
3. **Acceso a Poki**: el vault puede intentar abrirlo; si sale en blanco, es el bloqueo de Poki.

## Acceso a juegos en CodeTimeline

Triple clic en **© 2026** (footer) → abre el Game Vault.
No se añade nada al historial del navegador.
