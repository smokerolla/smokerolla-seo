---
title: Títulos SEO — 38 reescritos
key: 1hv4eiwz
---

# Títulos SEO reescritos

## Qué encontré (y qué corregí)

En un primer momento dije que tus títulos SEO **no estaban en Shopify** y que los generaba el tema. **Era falso.** Consulté el campo `metafields_global_title_tag` del objeto colección — un atajo heredado que casi nunca se rellena — y al verlo `null` saqué la conclusión equivocada.

Los títulos viven en **metafields**, que se piden aparte:

- `global.title_tag` — presente en **115 de 124** colecciones
- `global.description_tag` — presente en **115 de 124**

Verificado: en las 114 colecciones crawleadas, el metafield coincide **exactamente** con el `<title>` servido. Cero discrepancias. Son datos tuyos, editables, y sobreviven a cualquier cambio de tema.

## Sobre SEOKing (app ya desinstalada)

87 colecciones conservan un metafield `seoking.settings` **huérfano**. Shopify borra los datos privados de una app al desinstalarla, pero no los metafields que escribió. No se sirven al HTML y no afectan al SEO — son residuo. Limpiables cuando quieras; no urge.

Lo importante: **los títulos SEO no eran de SEOKing**, están en los metafields estándar `global.*` y siguieron funcionando tras desinstalarla. No había riesgo de que ninguna app revirtiera los cambios.

## Cambios aplicados

38 títulos superaban los 60 caracteres y Google los truncaba. Reescritos con la keyword al inicio y la marca solo cuando cabe. Todos verificados por API; comprobado en vivo que la web sirve los nuevos.

| Colección | Antes | Ahora | Keyword objetivo |
|---|---|---|---|
| `/bongs-water-pipes` | 68 ch | **41 ch** — Bongs & Water Pipes for Sale | Smokerolla | water bong |
| `/dab-rigs-oil-rigs` | 67 ch | **41 ch** — Dab Rigs & Oil Rigs for Sale | Smokerolla | dab rig |
| `/electric-dab-rigs` | 66 ch | **48 ch** — Electric Dab Rigs & E-Rigs for Sale | Smokerolla | electric dab rig |
| `/nectar-collectors-straws` | 62 ch | **43 ch** — Nectar Collectors & Dab Straws | Smokerolla | nectar collector |
| `/bong-bowls` | 68 ch | **46 ch** — Bong Bowls & Slides | 14mm & 18mm Replacements | bong bowls |
| `/ash-catchers` | 63 ch | **49 ch** — Ash Catchers for Bongs | 14mm & 18mm | Smokerolla | ash catcher |
| `/mini-bongs` | 64 ch | **43 ch** — Mini Bongs & Small Water Pipes | Smokerolla | mini bongs |
| `/herb-grinders` | 62 ch | **46 ch** — Herb Grinders | 2, 4-Piece & Electric Grinders | grinder weed |
| `/cute-and-girly-bongs-smoking-accessories` | 61 ch | **46 ch** — Cute & Girly Bongs | Pink & Pastel Glass Pipes | cute bongs |
| `/glass-blunts` | 66 ch | **46 ch** — Glass Blunts | Reusable Blunt Pipes, No Papers | glass blunt |
| `/percolator-bongs` | 61 ch | **46 ch** — Percolator Bongs | Tree & Honeycomb Perc Pipes | best percolator bongs |
| `/silicone-dab-rigs` | 63 ch | **41 ch** — Silicone Dab Rigs | Unbreakable Eyce Rigs | silicone dab rigs |
| `/electric-dab-nails` | 73 ch | **45 ch** — Electric Dab Nails & E-Nail Kits | Smokerolla | dab nail |
| `/recycler-bongs-dab-rigs` | 69 ch | **47 ch** — Recycler Dab Rigs & Bongs for Sale | Smokerolla | recycler dab rig |
| `/rolling-papers-wraps` | 64 ch | **44 ch** — Rolling Papers & Wraps | Hemp Papers & Cones | best rolling papers |
| `/smoking-kits` | 95 ch | **47 ch** — Smoking Kits & Bundles | Pipes, Grinders & More | — |
| `/hookahs` | 74 ch | **44 ch** — Hookahs & Shisha Pipes for Sale | Smokerolla | — |
| `/detox` | 73 ch | **46 ch** — Total Body Detox Kits & Cleansers | Smokerolla | — |
| `/bubblers` | 73 ch | **44 ch** — Glass Bubblers for Sale | Pocket Water Pipes | — |
| `/top-shelf` | 71 ch | **42 ch** — Top Shelf Smoking Accessories | Smokerolla | — |
| `/yocan` | 69 ch | **51 ch** — Yocan Vaporizers, Dab Pens & Batteries | Smokerolla | — |
| `/straight-tubes` | 69 ch | **47 ch** — Straight Tube Bongs | Classic Glass Water Pipes | — |
| `/smoking-accessories` | 69 ch | **46 ch** — Smoking Accessories | Bowls, Downstems & Parts | — |
| `/hand-pipes` | 68 ch | **45 ch** — Hand Pipes for Sale | Glass Spoons & Chillums | — |
| `/electric-herb-grinders` | 68 ch | **44 ch** — Electric Herb Grinders | Rechargeable & Auto | — |
| `/novelty-pipes` | 67 ch | **45 ch** — Novelty Pipes | Character & Themed Hand Pipes | — |
| `/hemp-blunt-wraps` | 67 ch | **45 ch** — Hemp Wraps | Tobacco-Free Blunt Wraps & Cones | — |
| `/dabbing-adapters` | 67 ch | **44 ch** — Bong & Dab Rig Adapters | 14mm & 18mm Joints | — |
| `/xvape` | 65 ch | **43 ch** — XVAPE Vaporizers | Vista Mini, Aria & Vital | — |
| `/ragabong` | 65 ch | **47 ch** — Ragabong Bamboo Bongs | Handcrafted Water Pipes | — |
| `/carb-caps` | 65 ch | **43 ch** — Carb Caps | Glass & Directional Banger Caps | — |
| `/blunt-wraps` | 65 ch | **43 ch** — Blunt Wraps | Flavored, Hemp & Tobacco-Free | — |
| `/titanium-ceramic-nails` | 64 ch | **41 ch** — Titanium & Ceramic Dab Nails | Smokerolla | — |
| `/25-off-cannabis-accessories-event` | 64 ch | **46 ch** — 25% Off Cannabis Accessories | Smokerolla Sale | — |
| `/vaporizers` | 63 ch | **41 ch** — Vaporizers | Dry Herb & Concentrate Vapes | — |
| `/pipes-under-25` | 62 ch | **40 ch** — Pipes Under $25 | Cheap Glass Hand Pipes | — |
| `/weedgets` | 61 ch | **41 ch** — Weedgets Smoking Accessories | Smokerolla | — |
| `/unicorn-dab-rigs` | 61 ch | **40 ch** — Unicorn Dab Rigs & Bongs | Lookah & More | — |

## Criterio de redacción

- **Keyword primero.** `/dab-rigs-oil-rigs` compite por "dab rig" (TP 31,000, KD 3): el título abre con eso, no con relleno.
- **La marca es opcional.** Se mantiene donde cabe bajo 60; se sacrifica antes que la keyword.
- **Fuera el ruido.** `/smoking-kits` pasó de 95 caracteres ("Smoking Accessories Bundled for Convenience & Savings - Shop Our Selection of Smoking Kits Now!") a 47.
- **Se conservan los cualificadores útiles**: "14mm & 18mm", "2, 4-Piece", "No Papers" — captan long tail real.

## Reversible

Los 38 títulos originales están guardados en `~/workspace/titles_backup.json`. Restaurar es reescribir el mismo metafield con el valor previo.

## Cabo suelto pendiente

`/collections/dab-rigs-oil-rigs` tiene un metafield `seo.hreflang_es_handle` → `dabbing-para-dab`, **colección que no existe**. Si el tema lo renderiza como `<link rel="alternate" hreflang="es">`, apunta a una URL rota. Queda por revisar si hay más casos.

← [[smokerolla-dtc-seo/shopify-findings]]
