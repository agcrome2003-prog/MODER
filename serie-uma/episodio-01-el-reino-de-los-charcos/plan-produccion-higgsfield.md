# Plan de producción en Higgsfield — Episodio 1

Notas para cuando pidas generar los videos de este episodio con Higgsfield
(`get_workflow_instructions({workflow:"faceless-video"})`). El propio pipeline te va a
volver a preguntar esto en su "intake" (no se puede saltar, ni siquiera en modo
"decide tú") — esta sección es para que las respuestas estén pensadas de antemano y la
producción no se frene a mitad de camino.

## ⚠️ Nota de alcance/costo antes de arrancar

Con el saldo actual (**1.210 créditos**, plan Plus), la producción completa es viable, pero
un episodio largo pesa: cada bloque de video de 10s es una llamada `minimax_h3` en 2K, más
las imágenes de estilo/assets, más narración, más música. El episodio largo (7–8 min) son
**42–48 bloques de 10s** — la producción más grande de las dos, ni cerca de agotar el saldo
pero sí la que más tarda y más llamadas hace.

**Recomendación:** producir primero el **Short** (5–6 bloques, ~1 min) como piloto — valida
estilo visual, voz del narrador y el diseño de Uma/Bibo en movimiento por una fracción del
costo — y con eso aprobado, lanzar el episodio largo completo. Decís vos si preferís ir
directo al episodio largo.

## Respuestas recomendadas para el intake (`faceless-video`, Fase 0)

| Pregunta del intake | Respuesta recomendada | Notas |
|---|---|---|
| Tipo de canal | **Kids** | — |
| Modo de movimiento | **Animado** | (10s de clips con cortes, no stills) |
| Quién lleva el sonido (solo Kids) | **Narrador + personajes que SÍ hablan** | Este show es más de diálogo (estilo sitcom familiar) que el Kids explicativo por defecto — el modo "narrador + personajes hablan" (Ronda 1c) le queda mejor. La opción "solo narrador" es la más económica/segura si preferís iterar primero con eso. |
| Estilo (galería de presets) | **Studio 3D** (alternativa: Colorful 3D) | Ver `00-biblia-de-la-serie.md` — paleta coral/melocotón/arena, evitando el azul como color dominante. |
| Duración — Short | **1 minuto** (5–6 bloques) | Guion ya escrito: `guion-corto-short.md`. |
| Duración — Episodio largo | **7–8 minutos** (Other → 7 u 8 min) | Guion ya escrito: `guion-largo.md`. |
| Aspecto | **9:16** para el Short · **16:9** para el largo | — |
| Subtítulos | **Sí** | Ayuda a la audiencia que mira sin sonido en Shorts. |
| Miniatura | **Sí** | — |
| De dónde sale el tema | **"Mi propio guion"** → pegar `guion-corto-short.md` o `guion-largo.md` | Son textos ya escritos por nosotros: el workflow los debe respetar palabra por palabra (no reescribir), solo partirlos en bloques. |
| Voz del narrador | Elegir en el selector (`list_voices`) una voz cálida en español | Aún no elegida — el pipeline abre la galería de voces para escuchar muestras antes de decidir. |

## Desglose en bloques — Short "El Monstruo del Charco" (~50s, 5 bloques × 10s)

Formato de cada bloque: 4 cortes duros de ~2.5s cada uno (patrón Kids:
GRAN PLANO general → PRIMER PLANO reacción → PLANO DETALLE → PLANO MEDIO resolución),
narración de 17–21 palabras por bloque.

**Bloque 1 — El charco misterioso**
> Narración: "Un charco grande y oscuro, escondido bajo las raíces. Y un niño que no piensa
> acercarse… ¡ni un poquitito!"
- SHOT 1 (0.0–2.5s) GRAN PLANO: el jardín después de la tormenta, el charco oscuro bajo las
  raíces del higuera.
- SHOT 2 (2.5–5.0s) PRIMER PLANO en Bibo: congelado, ojos bien abiertos, apuntando.
- SHOT 3 (5.0–7.5s) PLANO DETALLE: la superficie oscura del agua, algo se mueve debajo.
- SHOT 4 (7.5–10.0s) PLANO MEDIO: Bibo retrocede medio paso, abrazando a Ocho.

**Bloque 2 — El monstruo, según Bibo**
> Narración: "«¡Tiene ojos enormes, y dientes!», grita Bibo. Uma se agacha a su lado y le
> estira la mano con una sonrisa."
- SHOT 1 GRAN PLANO: Uma llega corriendo y se agacha junto a Bibo.
- SHOT 2 PRIMER PLANO en Bibo: gesticula "ojos grandes" con las manos, asustado.
- SHOT 3 PLANO DETALLE: la mano de Uma, extendida, esperando.
- SHOT 4 PLANO MEDIO: Bibo mira la mano, dudando.

**Bloque 3 — Vamos juntos**
> Narración: "«Yo también tengo miedo… ¿vamos juntos?», dice Uma. Bibo respira hondo y por
> fin toma su mano con fuerza."
- SHOT 1 PRIMER PLANO en Uma: honesta, cálida, sosteniendo la mirada de Bibo.
- SHOT 2 PLANO MEDIO: las dos manos se juntan.
- SHOT 3 GRAN PLANO: los dos caminan juntos hacia el borde del charco, muy despacio.
- SHOT 4 PLANO DETALLE: dos ojitos redondos parpadean en el agua oscura.

**Bloque 4 — El monstruo de verdad**
> Narración: "«¡Ahí está!», grita Bibo bajito. Pero Uma sonríe: «Bibo… mira bien» — no es
> ningún monstruo, es Mora, temblando de miedo."
- SHOT 1 PRIMER PLANO en Bibo: grito-susurro, señalando.
- SHOT 2 PLANO DETALLE: se revela a Mora, pequeñita, temblando detrás de una piedra.
- SHOT 3 PRIMER PLANO en Uma: sonríe, sin burla, señalando con la cabeza.
- SHOT 4 PLANO MEDIO: Bibo se asoma de verdad, sorprendido, cae en la cuenta.

**Bloque 5 — Una amiga nueva**
> Narración: "A veces, lo que más miedo nos da solo necesita un amigo. «Se llama Mora», dice
> Bibo, orgulloso, «y ya no es un monstruo»."
- SHOT 1 GRAN PLANO: entre los dos ayudan a Mora a subir al balde con agua.
- SHOT 2 PLANO MEDIO: sueltan a Mora en el mar, ella da una vuelta feliz.
- SHOT 3 PRIMER PLANO en Bibo: a cámara, orgulloso, sonriendo.
- SHOT 4 PLANO MEDIO final: Uma y Bibo se abrazan, la aleta de Mora asoma jugando cerca.

*(Cierre con cartel — no es un bloque de video, lo añade la Fase 8b si se pide miniatura /
cartel de cierre.)*

## Episodio largo — mapa de escenas a bloques (guía, no el desglose final)

La Fase 3 del propio workflow (`faceless-video`) es la que parte `guion-largo.md` en
bloques de 10s automáticamente al producirlo — no hace falta rehacer ese trabajo a mano
aquí. Como referencia de tamaño esperado:

| Sección del guion | Duración aprox. | Bloques aprox. (×10s) |
|---|---|---|
| Cold open + cartel de título | 40s | 4 |
| Acto 1 — La misión comienza (incl. montaje de rescates) | 1:35 | 9–10 |
| Acto 2 — El miedo de Bibo | 1:45 | 10–11 |
| Acto 3 — El Reino Azul Profundo | 1:45 | 10–11 |
| Cierre | 1:00 | 6 |
| **Total** | **~7:45** | **~42–45** |

## Personajes y assets a preparar (Fase 2 del workflow, cuando produzcamos)

- Personajes: Uma, Bibo (diseños ya aprobados en `personajes/referencias.md`), Papá Beto,
  Mamá Cami, Mora — Nano no aparece en este episodio.
- Localizaciones: jardín/casa-árbol Molano tras la tormenta, zona de raíces con el charco
  grande, la playa/orilla.
- Props recurrentes: los baldes "mágicos", el pulpo de peluche Ocho, la estrellita de mar.

## Próximo paso

Cuando quieras que arranque la producción real, decime: **short primero, episodio largo
primero, o los dos** — y arrancamos el intake de Higgsfield (galería de estilos + selector
de voz incluidos) para dejar todo bloqueado antes de generar el primer clip.
