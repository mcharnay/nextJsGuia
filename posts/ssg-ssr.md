---
title: 'Cuándo usar Static Generation v.s. Server-side Rendering'
date: '2023-03-13'
---

Recomendamos usar **Static Generation** (con o sin data) como sea posible, cuando tu página puede ser Buildeada una vez,  y servida con CDN, cuando la creas más rápido que teniendo un server render para la página en cada request.

You can use Static Generation for many types of pages, including:
PUedes usar Static Generation para muchos tupos de páginas incluyendo:

- Marketing pages
- Blog posts
- E-commerce product listings
- Help and documentation

Podrías preguntarte: ¿"Puedo pre-renderizar" esta página **adelante** de un user's request?. Si la respuesta es sí, entonces, deberías
elegir Static Generation.

Por otro lado, Static Generation **no** es buena idea si tu no puedes pre-render una página empezando una petición de usuario. Tal vez, tu página muestra data modificada constántementem y el contenido de la página cambia en cada petición.

En ese caso, puedes user **Server-Side Rendering**. Será lento, pero, la página pre-rendereada siempre estára al día. O, puedes adelantar
pre-rendering y user Javascript client-Side para poblar data.