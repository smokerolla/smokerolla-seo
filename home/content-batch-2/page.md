---
title: Contenido ampliado — 8 colecciones más
key: 1ek570j1
---

# Segundo lote de contenido

Tras llenar las colecciones de productos, les tocaba contenido. **Cinco ampliadas** (ya tenían el patrón correcto) y **tres reescritas** (no lo tenían).

## Ampliadas — se respetó lo existente

Estas ya tenían la estructura `srcol` con FAQ. No las reescribí: **inserté secciones nuevas antes del bloque FAQ y añadí preguntas al final**, conservando intacto el texto y los enlaces a producto que ya había.

| Colección | Texto antes | **Ahora** | Añadido |
|---|---:|---:|---|
| `/carb-caps` | 2,312 ch | **4,375 ch** | Técnica de uso · Materiales · 4 FAQ |
| `/bong-bowls` | 2,178 ch | **4,224 ch** | Tamaño de bowl · Cuándo reemplazar · 4 FAQ |
| `/straight-tubes` | 2,282 ch | **3,632 ch** | Straight tube vs beaker · 3 FAQ |
| `/blunt-wraps` | 2,352 ch | **3,617 ch** | Materiales de wrap · 3 FAQ |
| `/mini-bongs` | 2,353 ch | **3,577 ch** | Qué ganas y qué pierdes · 3 FAQ |

## Reescritas desde cero

Estas tres no seguían el patrón y no tenían FAQ:

| Colección | Productos | Texto | Contenido |
|---|---:|---:|---|
| `/best-wax-vaporizers-oil-vapes` | 44 | **3,163 ch** | Tipos de coil · Wax pen vs dab rig · 4 recomendaciones · 5 FAQ |
| `/titanium-ceramic-nails` | 3 | **3,223 ch** | Titanio vs cerámica vs cuarzo · Uso correcto · 5 FAQ |
| `/dual-use-vaporizers` | 6 | **2,946 ch** | Qué significa dual-use · ¿Basta un dispositivo? · 4 FAQ |

## Dos problemas técnicos detectados y resueltos

**1. Schema FAQ desincronizado.** Al añadir preguntas nuevas al HTML, el bloque `FAQPage` seguía listando solo las 5 originales — Google habría visto 5 de 9. Regenerado desde los pares pregunta/respuesta reales del cuerpo. Verificado: HTML y schema coinciden en las ocho páginas.

**2. Schema FAQPage duplicado.** Descubierto al verificar: **tu tema ya genera `FAQPage` automáticamente** a partir de los `<h3>` bajo "Frequently asked questions". Mi script añadía un segundo bloque idéntico, así que cinco páginas servían el mismo FAQ dos veces — algo que Google puede interpretar como marcado manipulado.

Lo detecté comparando con `/herb-grinders`, que también daba 2. **Eliminados mis scripts redundantes** de las cinco páginas afectadas. Ahora todas sirven exactamente uno.

Vale la pena señalarlo: el error venía de asumir que el tema no hacía nada. Hacía bastante.

## Un falso positivo más del etiquetado

`/titanium-ceramic-nails` mostraba un *"Ak-47 Dab Straw - Food Grade Silicone With Titanium Tip"*. Tiene "Titanium" en el título, pero es un nectar collector de silicona, no un nail. Etiqueta retirada — la colección queda en 3 productos correctos.

## Estado del contenido

Trece colecciones con contenido completo, FAQ schema válido y sin duplicados:

`herb-grinders` · `dab-rigs-oil-rigs` · `nectar-collectors-straws` · `bongs-water-pipes` · `ash-catchers` · `terp-slurpers` · `electric-dab-rigs` · `dry-herb-vaporizers` · `vape-pens` · `percolator-bongs` · `quartz-bangers-nails` · `grav` · más las ocho de esta tanda.

## Reversible

Todos los cuerpos anteriores en `~/workspace/bodies_backup.json`.

← [[smokerolla-dtc-seo/bulk-retag]] · [[smokerolla-dtc-seo/collection-content]]
