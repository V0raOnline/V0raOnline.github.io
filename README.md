# V0raOnline.github.io

Homepage y catálogo. Se publica en la **raíz** de `https://v0raonline.github.io/`,
que es el único sitio donde un `robots.txt` cuenta para todos los proyectos
alojados en ese subdominio.

## Contenido

| Archivo | Para qué |
|---|---|
| `index.html` | Catálogo: herramientas con demo, repos sin demo, enlace a Substack. Autocontenido, sin dependencias externas. |
| `robots.txt` | Reglas de rastreo para **todo** `v0raonline.github.io`, subproyectos incluidos. |
| `sitemap.xml` | Lista de URLs para los buscadores. Referenciado desde `robots.txt`. |

## Política de `robots.txt`

Abierto a lo que **cita con enlace**, cerrado a lo que solo **absorbe**:

- **Permitidos** — buscadores clásicos (Googlebot, bingbot, DuckDuckBot, Applebot)
  y bots de búsqueda con IA que devuelven fuente clicable (OAI-SearchBot,
  ChatGPT-User, Claude-SearchBot, Claude-User, PerplexityBot, Perplexity-User).
- **Bloqueados** — rastreadores de entrenamiento (GPTBot, ClaudeBot, CCBot,
  Google-Extended, Applebot-Extended, Bytespider, meta-externalagent y compañía).

Dos avisos permanentes:

1. `robots.txt` es una petición, no una valla. Los grandes la respetan; un
   scraper anónimo se la salta. Lo que no deba leerse, no se publica.
2. **No cubre Substack.** Es otro dominio con sus propias reglas; el bloqueo de
   IA se activa en los ajustes de la publicación, no aquí.

## Publicar

`Settings → Pages → Deploy from a branch → main / (root)`.
Tarda uno o dos minutos en estar vivo.

## Mantenimiento

Cuando un proyecto nuevo estrene Pages, tocar tres sitios: una tarjeta en
`index.html`, una `<url>` en `sitemap.xml` y el bloque JSON-LD del final de
`index.html`.
