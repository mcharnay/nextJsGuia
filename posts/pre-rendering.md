---
title: 'Dos formas de Pre-rendering'
date: '2023-03-13'
---

Next.js tiene dos formas de pre-renderizar: **Static Generation** y **Server-side Rendering**. La diferencia está en **Dónde** esto genera el
HTML para una página.

- **Static Generation** es el método pre-renderización que genera el HTML en **build time**. El HTML pre-rederizado es entonces, _reutilizado_ en cada request.

- **Server-side Rendering** es el método pre-rederizando que genera el HTML en cada request.

Importantemente, Next.JS, te va a hacer **elegir** cual forma pre-renderizada vas a usar en cada página. Puedes crear una aplicación "Híbrida"
usando Static Generation para más páginas y usando Server-side Rendering para otras.