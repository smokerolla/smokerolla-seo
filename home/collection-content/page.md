---
title: Contenido de colecciones — 5 páginas reescritas
key: 1uyovyi1
---

# Contenido de colecciones completado

Cinco colecciones tenían el título arreglado pero el cuerpo a medias. Reescritas siguiendo **tu propio patrón**, el de `/collections/herb-grinders` — que es tu mejor página y ya tenía la estructura correcta.

## Error corregido antes de escribir

Al auditar el contenido detecté un fallo **en mi propio etiquetado de la sesión anterior**: había metido **14 accesorios en colecciones de dispositivos**. Bobinas de repuesto, boquillas, carb caps y collares de recambio aparecían como si fueran e-rigs o vaporizadores:

- *Pulsar Rök Electric Dab Rig Replacement Ceramic Coils* → etiquetado como vaporizador de hierba seca
- *Lookah Unicorn E-Rig Quartz Coil Set* → etiquetado como e-rig
- *Yocan iCan E-Rig Airflow Carb Cap* → etiquetado como e-rig

Mi filtro buscaba coincidencias de título, y "E-Rig Replacement Coils" contiene "e-rig". Un cliente que entrara a comprar un dab rig eléctrico se habría encontrado bobinas de repuesto entre los productos.

**Revertido.** Conteos corregidos:

| Colección | Antes de revertir | **Corregido** |
|---|---:|---:|
| `electric-dab-rigs` | 37 | **24** dispositivos reales |
| `dry-herb-vaporizers` | 32 | **31** |

Menos productos, pero todos correctos. Una colección con 24 dispositivos reales convierte mejor que una con 37 donde 13 son recambios.

## Contenido publicado

Las cinco páginas llevan ahora la misma estructura que `/herb-grinders`:

| Colección | Texto antes | **Ahora** | Bloques |
|---|---:|---:|---|
| `/dry-herb-vaporizers` | 2,344 ch | **3,351 ch** | Guía de compra · Vapear vs fumar · 4 recomendaciones · 5 FAQ |
| `/vape-pens` | 1,635 ch | **3,243 ch** | Cómo elegir · 510 vs todo-en-uno · 4 recomendaciones · 5 FAQ |
| `/percolator-bongs` | 2,510 ch | **3,199 ch** | Tipos de perc · Qué cambia · 4 recomendaciones · 5 FAQ |
| `/quartz-bangers-nails` | 2,780 ch | **3,252 ch** | Medidas y encaje · Estilos · 4 recomendaciones · 5 FAQ |
| `/grav` | 258 ch | **~3,200 ch** | Qué distingue a GRAV · 6 recomendaciones · 5 FAQ |

Todas con **FAQPage schema** y **CollectionPage schema** — verificado en vivo, los cinco sirven `FAQPage` correctamente.

## Keywords que persigue el contenido nuevo

El texto no es relleno: cada bloque va a por consultas concretas de la shortlist y de sus long tails.

| Página | Keyword principal | Long tails atacadas en el cuerpo |
|---|---|---|
| dry-herb-vaporizers | cannabis vaporizer (TP 35,000, KD 0) | "what temperature vape dry herb", "vaporizer vs smoking", "do dry herb vaporizers smell" |
| vape-pens | vape pen / 510 battery | "what is a 510 thread vape pen", "what voltage for cartridge", "why is my vape pen not hitting" |
| percolator-bongs | best percolator bongs (KD 2) | "what does a percolator do", "which perc type is best", "how to clean a percolator bong" |
| quartz-bangers-nails | dab banger (TP 3,200, KD 0) | "what temperature quartz banger", "14mm or 18mm", "banger vs nail", "why is my banger cloudy" |
| grav | grav bong (TP 65,000, KD 2) | "is grav glass worth it", "what is grav known for", "grav joint size" |

Las preguntas de los FAQ están redactadas como consultas reales de búsqueda, con respuestas directas en la primera frase — el formato que Google usa para fragmentos destacados y que los buscadores con IA citan.

## Títulos y metas añadidos

Tres de estas páginas no entraban en el lote de los 38 porque sus títulos no superaban los 60 caracteres — pero eran malos igualmente (`Vape Pens: Shop the Collection` no persigue nada). Reescritos:

- `Dry Herb Vaporizers | Portable & Desktop Vapes` (46 ch)
- `Vape Pens & 510 Batteries | Wax & Oil Pens` (42 ch)
- `Quartz Bangers & Nails | 14mm & 18mm | Smokerolla` (49 ch)

Más sus meta descriptions correspondientes.

## Verificación de enlaces

El primer borrador contenía **15 enlaces a productos inexistentes** — escribí los handles de memoria a partir de los títulos (`yocan-hit-2-portable-dry-herb-vaporizer`) cuando el real era `yocan-hit-2-herbal-vape-device`. Comprobados todos contra el catálogo antes de publicar; **cero enlaces rotos** en las cinco páginas.

## Reversible

Los cinco cuerpos originales están en `~/workspace/bodies_backup.json`.

← [[smokerolla-dtc-seo/internal-links]] · [[smokerolla-dtc-seo/priority-shortlist]]
