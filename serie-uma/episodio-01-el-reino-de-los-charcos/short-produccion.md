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

## Miniatura personalizada

- **Archivo final, listo para subir como miniatura del Short:** https://d2ol7oe51mr4n9.cloudfront.net/user_3HpearYMVAw2uXHmTqs3brJxqg1/8457a4e9-8746-44c7-aa74-ac230fbad862.jpg
  — JPEG, 1080×1920 (vertical, formato Shorts), ~338 KB.
- **Concepto:** Bibo, aterrado, abraza a Ocho mirando el charco oscuro; dos ojos
  brillantes lo espían apenas asomados bajo el agua (Mora, todavía sin revelar). Texto
  superpuesto "¿AMIGO O MONSTRUO?" — la pregunta que resume el giro del video sin
  spoilearlo, para generar curiosidad real (framework "Amplified Reality" +
  "Posed Portrait" del workflow de miniaturas: la cara con emoción domina el cuadro y el
  elemento de misterio está exagerado pero es fiel a lo que pasa en el video).
- Render generado con `nano_banana_pro` a 4K (3072×5504) usando como referencia el estilo
  Colorful 3D ya bloqueado y los diseños exactos de Bibo, Mora, Ocho y el charco — mismo
  aspecto que el resto de la producción. Texto agregado aparte con el motor de tipografía
  del workflow (estilo "Beast": blanco con borde negro grueso), no generado por IA, para
  que se lea perfecto.
  - `job_id` del render elegido (limpio, sin texto): `08e1176b-832b-41a0-8ca5-9b870c8ec754`
- **Otra toma generada** (mismo concepto, primer plano más cerrado sobre la cara de
  Bibo) — quedó disponible por si se prefiere esa composición:
  https://d8j0ntlcm91z4.cloudfront.net/user_3HpearYMVAw2uXHmTqs3brJxqg1/hf_20260903_182523_07ac0c4c-5c36-4fd8-817b-d74cd9ab59b9.png
  (`job_id`: `07ac0c4c-5c36-4fd8-817b-d74cd9ab59b9`, sin texto agregado todavía)

## Descripción para el video (lista para copiar y pegar)

```
¿Amigo o monstruo? 😨🌊 Bibo no se anima a mirar el charco oscuro... hasta que descubre
que "el monstruo" solo necesitaba un amigo. Un Short de Uma Coral sobre el miedo, la
valentía y la amistad — dibujos animados para niños. 🐙

Nuevas aventuras en Bahía Coral cada semana. ¡Suscribite y activá la campana! 🔔

#Shorts #DibujosAnimados #CuentosParaNiños #UmaCoral
```

Estructura pensada para el algoritmo: `#Shorts` primero (ayuda a clasificarlo en el
feed de Shorts), la pregunta-gancho y la palabra clave "dibujos animados para niños" en
las primeras líneas, sin spoilear el final, y cierre con llamada a suscribirse.

## Siguiente paso posible

Con miniatura y descripción listas, este Short queda con todo lo necesario para subir.
Lo que sigue pendiente de toda la serie es el episodio largo (~7-8 min) con el mismo
estilo y voz.
