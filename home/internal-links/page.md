---
title: Enlaces internos + colección GRAV
key: 48an0phw
---

# Enlaces internos hacia colecciones huérfanas

La auditoría encontró **50 colecciones sin un solo enlace desde el blog**, entre ellas todas las de marca. Esto lo corrige donde había contexto real para hacerlo.

## Criterio: solo enlaces que ya tenían sentido

No inserté enlaces forzados. El método fue buscar posts que **ya mencionaban** el término en prosa y no enlazaban a ninguna parte, y convertir esa primera mención en enlace. Descartes automáticos:

- Menciones dentro de `alt=`, `src=` o cualquier atributo HTML
- Texto dentro de encabezados, tablas, `figure` o `figcaption`
- Menciones ya enlazadas
- Posts que ya apuntaban a esa colección
- **Máximo 2 enlaces nuevos por post**

De 50 candidatos iniciales, 15 se descartaron por estos filtros. Quedaron **35 enlaces en prosa real**.

## Aplicado

| Colección destino | Enlaces antes | Ahora |
|---|---:|---:|
| `/collections/puffco` | 0 | **16** |
| `/collections/buy-pulsar-vaporizers-premium-vapes` | 0 | **5** |
| `/collections/dab-rigs-under-50` | 0 | **4** |
| `/collections/glow-in-the-dark-bongs` | 0 | **4** |
| `/collections/spoon-pipes` | 0 | **3** |
| `/collections/gas-mask-bongs` | 0 | **1** |
| `/collections/steamroller-pipes` | 0 | **1** |
| `/collections/raw` | 0 | **1** |

Ejemplo real, en `rokin-stinger-review-2026`:

> "Skip it if: you prefer big chamber-style e-rigs or already own a **[Puffco Peak Pro](/collections/puffco)**."

La mención ya estaba escrita; solo faltaba que llevara a alguna parte.

## Colección GRAV creada

`grav bong` puntuó **TP 65,000 con KD 2** — el mejor objetivo de toda la shortlist. Al revisar el catálogo:

- **16 productos GRAV en stock** (water pipes, bubblers, spoon pipes, bowls)
- Un post dedicado ya publicado: `/blogs/brands/grav-labs-precision-scientific-glass-since-2004`
- **Ninguna colección donde comprarlos**

Creada **[/collections/grav](https://smokerolla.com/collections/grav)** — smart collection sobre la etiqueta `Cat_Grav` (16 productos etiquetados), con título y meta SEO propios:

- `GRAV Glass | Scientific Bongs, Bubblers & Pipes` (47 caracteres)
- Verificada en vivo: HTTP 200, sirviendo el título correcto

## Marcas sin colección y sin inventario

Revisé el resto de marcas con alta puntuación. **No todas son accionables:**

| Marca | TP | Productos en stock | Veredicto |
|---|---:|---:|---|
| GRAV | 65,000 | 16 | ✅ Colección creada |
| King Palm | 15,000 | 4 | Poco surtido — decisión de compras |
| Hamilton Devices | 6,800 | **0** | No lo distribuyes |
| Bear Quartz | 1,300 | **0** | No lo distribuyes |
| MAV Glass | 1,200 | 3 | Marginal |

Hamilton Devices y Bear Quartz salían con KD 0 en el análisis de keywords, pero **no tienes producto**. Rankear por una marca que no vendes no sirve de nada: eso es una decisión de distribución, no de SEO.

## Reversible

Los 35 cuerpos de artículo originales están en `~/workspace/articles_backup.json`. La colección GRAV se elimina borrando la smart collection y la etiqueta `Cat_Grav`.

## Lo que sigue sin resolverse

Los enlaces internos redistribuyen la autoridad que ya tienes. **No la crean.** Tus colecciones siguen con una mediana de **0 dominios de referencia** — eso solo se mueve con enlaces externos, y es un trabajo distinto.

← [[smokerolla-dtc-seo/seo-titles]] · [[smokerolla-dtc-seo/priority-shortlist]]
