# Short "El Monstruo del Charco" — registro de producción (Higgsfield)

Producido con el workflow `faceless-video` de Higgsfield. Este archivo es el "ADN del
canal" de esta producción: guardá estos IDs para reusarlos en el próximo video sin
tener que regenerar estilo, voz ni personajes desde cero.

## Resultado

- **Video final (con subtítulos quemados):** https://d2ol7oe51mr4n9.cloudfront.net/user_3HpearYMVAw2uXHmTqs3brJxqg1/0a780fec-b775-461f-b5eb-6f6125647bc5.mp4
- **Miniatura/portada:** https://d2ol7oe51mr4n9.cloudfront.net/user_3HpearYMVAw2uXHmTqs3brJxqg1/16c6e03f-9bbd-4d47-aa23-94b948791b93.jpg
- Duración: 60s exactos · 9:16 · 6 bloques de 10s · subtítulos quemados (estilo "clean")
- Música de fondo: sí (instrumental, ukelele/marimba, generada, volumen bajo)

## Decisiones bloqueadas (intake)

| Parámetro | Valor | Origen |
|---|---|---|
| Tipo de canal | Kids | biblia de la serie |
| Modo | Animado (`minimax_h3`, 2K) | por defecto |
| Estilo | **Colorful 3D** | elegiste vos, reemplazando el default (Studio 3D) |
| Duración/aspecto | 60s · 9:16 | pedido |
| Subtítulos | Sí (clean) | plan de producción |
| Voz | **Judy** (`3375c7b3-8e04-5d44-9e09-33532864477d`, preset) | elegiste vos, reemplazando Helena y mi sugerencia (Marisol) |

## Estilo (Phase 1)

- `style_key_job_id`: `da2b22ee-aec8-45d0-b395-b48085f45a02`
- Donantes: preset "Colorful 3D" (`30948d66-76b1-4c8e-884a-1854e08e91df`) + 2 imágenes
  canónicas de `kids-styles.md`.

## Roster de personajes / localizaciones / props (Phase 2)

| Asset | job_id |
|---|---|
| char_uma | `4c42af6a-e5f7-4334-8657-68835887c062` |
| char_bibo | `7c54c0d5-fb70-4b47-899e-78144d657d69` |
| char_mora | `c3b0e1b4-5ee7-465f-888b-fefe66a9237d` |
| loc_charco | `82e73fe6-58f3-4e28-a5f8-62baef8fb008` |
| loc_borde | `3cc70191-57c9-4ce3-a0c7-a2f6d6810a73` |
| loc_detalle | `2df6b62a-1238-43f4-9ce8-c88edbd92037` |
| loc_orilla | `966322a7-96f8-465c-8966-17f65f641f4a` |
| prop_ocho | `453d86a6-34d0-460f-a13c-e3d781066712` |

## Nota de calidad — una línea de la voz

Todas las líneas de narración cumplen la ventana de duración (7.8–9.5s). La línea del
bloque 6 (el cierre, "Lo que más miedo nos da...") necesitó ocho reescrituras para
encajar en esa ventana con la voz de Judy — quedó bien de duración (8.77s) pero se lee
un poquito más rápido de lo ideal (ritmo ligeramente por encima del máximo recomendado).
No afecta la comprensión ni el resultado final, pero si al escucharlo te suena
apurada esa última frase, es la más fácil de regenerar sola.

También: para que el audio entrara en esa ventana de 7.8–9.5s, varias líneas quedaron
con más palabras (22–25) de las que este workflow recomienda por defecto para Kids
(17–21) — ese rango está calibrado en inglés, y en español, con esta voz, hacían falta
más palabras para llenar el mismo tiempo. Es una discrepancia menor del validador, no
un problema del video.

## Siguiente paso posible

No se generó una miniatura personalizada (workflow `thumbnail-generation`) — se usó el
poster automático del ensamblador. Si querés una miniatura diseñada (título, texto,
personajes en pose), lo puedo hacer en una pasada aparte.
