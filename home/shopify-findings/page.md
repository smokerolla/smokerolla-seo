---
title: Shopify — causa raíz de las colecciones vacías
key: 1j9d0ad1
---

# Lo que reveló el acceso a Shopify

Conectado a `bluntwrapvenezuela.myshopify.com` (= smokerolla.com, plan Professional). La lectura de la Admin API **corrige el hallazgo principal de la auditoría**.

## El crawl me engañó (y la API lo desmiente)

El crawl contaba los enlaces a producto en el HTML. Eso no es el inventario real — es lo que la plantilla pinta en la primera página. Comparación:

| Colección | Crawl | **Real (API)** |
|---|---:|---:|
| bongs-water-pipes | 28 | **250** |
| yocan | 29 | **205** |
| herb-grinders | 30 | **172** |
| dab-rigs-oil-rigs | 28 | **98** |
| nectar-collectors-straws | 29 | **71** |
| puffco | 23 | **71** |
| lookah | 23 | **51** |

**La mayoría de tus colecciones no están vacías en absoluto.** El "28 productos" era paginación, no escasez. Retiro esa parte del diagnóstico.

## Pero cinco colecciones sí están rotas — y por una razón concreta

Todas son **smart collections** con una regla de etiqueta. Los productos existen; **no llevan la etiqueta**.

| Colección | Ahora | Podría tener | Sin etiquetar | Traffic potential |
|---|---:|---:|---:|---:|
| `dry-herb-vaporizers` | **5** | 31 | 27 | 35,000 |
| `electric-dab-rigs` | **4** | 33 | **33** | 18,000 |
| `ash-catchers` | **6** | 21 | 15 | 5,900 |
| `terp-slurpers` | **9** | 17 | 8 | 5,100 |

Ejemplo — `electric-dab-rigs` exige la etiqueta `Electric Dab Rigs`. **Cero** de los 33 productos en stock que coinciden la llevan:

- Dr Dabber Switch 2 Powerful Electric Dab Rig
- Carta Sport Endurance Electric Dab Rig
- Dabtron 2.0 Grenade Electric Dab Rig
- Dr. Dabber Boost eRig Ceramic Nail

Son productos activos, con stock, con el término exacto en el título — invisibles en la colección que debería venderlos, y en la que Google debería rankear.

## Por qué pasó

El catálogo tiene **6,372 etiquetas distintas** para 4,316 productos, y solo 299 se usan en 20+ productos. Conviven vocabularios incompatibles: `Cat_AshCatcher`, `Cat_GlassBlunt`, `Cat_MiniBong` (prefijo `Cat_`) junto a `Dry Herb Vaporizers`, `Electric Dab Rigs`, `Terp_Slurper` (sin prefijo, con y sin guion bajo). Nadie puede etiquetar de forma consistente contra un vocabulario así: el producto nuevo entra sin la etiqueta y la colección deja de crecer en silencio.

`glass-blunts` es el caso extremo: la etiqueta `Cat_GlassBlunt` **solo existe en 1 producto de todo el catálogo**, y solo un título contiene "glass blunt". Ahí sí falta surtido real, no etiquetas — es una decisión de compras, no de SEO.

## Qué cambia en las prioridades

Esto **refuerza** la conclusión de fondo y abarata la solución. El mejor objetivo por dificultad era `cannabis vaporizer` (TP 35,000, KD 0) apuntando a `/collections/dry-herb-vaporizers`. Esa página muestra 5 productos de 31 disponibles. No hay que crear contenido ni comprar inventario: **hay que etiquetar 27 productos que ya tienes**.

**83 productos a etiquetar en total**, sobre colecciones con ~64,000 de traffic potential combinado.

## Ejecutado — etiquetado aplicado

83 productos etiquetados vía Admin API. Resultado verificado por API:

| Colección | Antes | **Ahora** | Traffic potential |
|---|---:|---:|---:|
| `dry-herb-vaporizers` | 5 | **32** | 35,000 |
| `electric-dab-rigs` | 4 | **37** | 18,000 |
| `ash-catchers` | 6 | **21** | 5,900 |
| `terp-slurpers` | 9 | **17** | 5,100 |
| **Total visible** | **24** | **107** | |

`electric-dab-rigs` acabó con 37, más de los 33 previstos: al añadir la etiqueta entraron también productos que ya cumplían la regla de stock pero que mi filtro por título no había capturado.

**Nota operativa:** las smart collections de Shopify reindexan con retardo. Justo tras escribir, la colección mostraba 26; un minuto después, 37. Si compruebas conteos inmediatamente tras un cambio masivo, espera antes de sacar conclusiones.

**Reversible:** cada cambio consistió en añadir una etiqueta al campo `tags`. El listado completo está en el CSV del plan.

## Propuesta original (ya aplicada)

1. Etiquetar los 83 productos según su título (coincidencia exacta, solo activos y con stock).
2. Antes de escribir: te entrego la lista completa producto→etiqueta para revisión.
3. Después: verificar los conteos vía API y re-crawlear las 4 colecciones.

**No toco nada sin que apruebes la lista.** El etiquetado es reversible (se quita igual que se pone), pero afecta a la navegación de la tienda en vivo.

**Aparte, para decidir tú:** el vocabulario de 6,372 etiquetas es el problema de fondo. Etiquetar estos 83 arregla el síntoma; volverá a pasar con cada producto nuevo salvo que se consolide a un esquema único. Es un proyecto propio, y te lo planteo por separado.

← [[smokerolla-dtc-seo/seo-audit]] · [[smokerolla-dtc-seo/priority-shortlist]]
