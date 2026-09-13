---
title: Tercer lote — colecciones y enlaces restantes
key: mdmk61vc
---

# Tercer lote: lo que quedaba

## Colecciones: 64 → 112 productos

Once colecciones más llenadas. Pero el mecanismo fue distinto al de las tandas anteriores, y ahí estuvo el aprendizaje.

| Colección | Antes | **Ahora** |
|---|---:|---:|
| `/vape-pens` | 8 | **28** |
| `/glass-adapters` | 7 | **14** |
| `/smell-proof-storage` | 1 | **12** |
| `/unicorn-dab-rigs` | 8 | **12** |
| `/skull-bongs` | 4 | **7** |
| `/electric-dab-nails` | 6 | **7** |
| `/electric-herb-grinders` | 4 | **5** |
| `/steamroller-pipes` | 4 | **5** |

## Por qué el primer intento no funcionó

Etiqueté 80 productos y **solo 4 colecciones se movieron**. Al investigar: estas colecciones no usan reglas de etiqueta, sino **reglas por título** — `/vape-pens` incluía únicamente productos cuyo título contiene literalmente "vape pen".

Eso explica por qué estaban vacías: tu catálogo tiene 25 baterías 510 en stock con nombres como *"Caligo REAKT Precision 510 Vape Battery"* — ninguna dice "vape pen", así que ninguna entraba.

**Solución en dos pasos**, para no perder nada:

1. Etiquetar primero los productos **que ya estaban** en cada colección (para que la nueva regla sea un superconjunto de la antigua).
2. Cambiar la regla de `title contains` a `tag equals`.

Reglas anteriores guardadas en `~/workspace/rules_backup.json`. Siete colecciones migradas así.

## Filtrado por product_type

En esta tanda añadí un filtro que faltaba: **el tipo de producto**. Sin él, `/skull-bongs` iba a recibir una *camiseta "Cannabis Skull"* y un *tapiz de pared de 3ft x 2ft* — ambos con "skull" en el título. Restringiendo a `Bongs & Water Pipes`, `Hand Pipes`, `Dab Rigs` y `Beaker Bong`, quedaron solo los 3 correctos.

También descarté tres *"Arizer Power Adapter"* y *"In-Vehicle Power Adapter"* de `/glass-adapters`: son cargadores, no adaptadores de junta.

## Enlaces internos: 62 más

Aplicados sobre 58 artículos, con el mismo criterio de siempre — solo menciones ya existentes en prosa.

| Destino | Enlaces |
|---|---:|
| `/ooze` | 8 |
| `/santa-cruz-shredder` | 8 |
| `/storz-bickel` | 6 |
| `/dabbing-adapters` | 6 |
| `/filtration` | 6 |
| `/g-pen` · `/pipes-under-25` · `/unicorn-dab-rigs` | 5 c/u |

**Un límite que me puse:** "adapter" y "filtration" aparecían 63 y 52 veces respectivamente en el blog. Enlazar todas habría sido spam de enlaces internos — el patrón que Google penaliza. **Capé a 6 por destino.** Un enlace interno vale por su contexto, no por su cantidad; 63 enlaces con el mismo anchor hacia la misma página no valen más que 6 bien colocados.

## Estado de las colecciones huérfanas

De 50 iniciales quedan **~20 sin enlaces**, y la mayoría son casos donde no hay contexto natural en el blog: `/mob-hookah`, `/hookah-charcoal`, `/afghan-hemp`, `/weedgets`. Escribir menciones artificiales para enlazarlas sería exactamente el tipo de contenido que no funciona.

Para esas, la vía correcta es contenido nuevo que las cubra de verdad — no forzar enlaces en posts que hablan de otra cosa.

## Reversible

- Etiquetas: `~/workspace/tags_backup3.json`
- Reglas de colección: `~/workspace/rules_backup.json`
- Artículos: `~/workspace/articles_backup2.json`

← [[smokerolla-dtc-seo/content-batch-2]] · [[smokerolla-dtc-seo/internal-links]]
