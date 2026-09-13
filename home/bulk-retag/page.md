---
title: Etiquetado masivo — 10 colecciones más
key: 1ww7h1sb
---

# Segundo lote de etiquetado

Extendido el arreglo de etiquetas al resto de colecciones infradotadas. **51 productos etiquetados**, tras descartar 143 que ya estaban correctos.

## Resultado

| Colección | Antes | **Ahora** |
|---|---:|---:|
| `/best-wax-vaporizers-oil-vapes` | 2 | **44** |
| `/bong-bowls` | 14 | **59** |
| `/quartz-bangers-nails` | 5 | **38** |
| `/carb-caps` | 5 | **27** |
| `/straight-tubes` | 13 | **25** |
| `/mini-bongs` | 10 | **17** |
| `/blunt-wraps` | 10 | **11** |
| `/dual-use-vaporizers` | 1 | **6** |
| `/titanium-ceramic-nails` | 2 | **4** |
| **Total** | **65** | **234** |

`/best-wax-vaporizers-oil-vapes` pasó de 2 productos a 44 — perseguía "wax vape" (vol 1,000) con una colección prácticamente vacía.

## Tres errores detectados antes de publicar

**1. "Bong con bowl" no es un bowl.** Mi primer filtro dio 145 productos para `/bong-bowls` porque capturaba cualquier título con la palabra "bowl" — incluidos bongs de 10 pulgadas *que incluyen* un bowl de 14mm. Solución: analizar únicamente la parte del título **anterior** a "with" / "and" / "&", ya que lo que va después es un accesorio, no el producto. De 145 pasó a 48 reales.

**2. Lo mismo con bangers.** "8 Ball Borosilicate Dab Rig **with Banger**" es un rig, no un banger. Mismo arreglo.

**3. Revisión manual sobre muestra aleatoria.** Inspeccioné 4 productos al azar por colección antes de escribir, y salieron falsos positivos que ninguna regex había filtrado: un *"LEAF Blue Slide Glass Hand Pipe"* iba a entrar en bong-bowls (dice "slide", pero es una pipa), y un *"Silicone Magnetic Cleaner"* en silicone-dab-rigs. Excluidos.

## Un caso donde la regla tenía razón y yo no

`/silicone-dab-rigs` no se movió pese a etiquetar 12 productos. Al investigar, su regla exige **dos** condiciones: la etiqueta `Material_Silicone` **y** `product_type = "Dab Rigs"`.

Consulté el `product_type` de los 12: cinco eran "Bongs & Water Pipes", tres "Hand Pipes", tres "Smoking Accessories", uno "Bong Bowls". **Ninguno era un dab rig.** Mi filtro por título capturaba cualquier cosa de silicona; la regla de la colección era más estricta y más correcta.

**Las 12 etiquetas revertidas.** La colección sigue con 3 productos, y ese es el número honesto: no tienes más dab rigs de silicona en stock. Forzarla habría llenado de pipas una colección que promete rigs.

Vale la pena señalarlo porque contradice el patrón de toda la sesión: aquí la configuración existente era correcta y mi automatización la habría degradado.

## Reversible

Etiquetas previas de los 194 productos evaluados en `~/workspace/tags_backup2.json`.

← [[smokerolla-dtc-seo/collection-content]] · [[smokerolla-dtc-seo/shopify-findings]]
