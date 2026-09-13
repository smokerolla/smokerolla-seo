---
title: Auditoría de backlinks — spam detectado
key: 1fsm0d55
---

# Auditoría del perfil de enlaces

**Sí hay spam, y es reciente.** Pero antes del diagnóstico, el contexto que evita el pánico.

## Estado general

| Métrica | Actual | Histórico |
|---|---:|---:|
| Dominios de referencia | **564** | 1,743 |
| Backlinks | **1,106** | 8,230 |

**1.96 enlaces por dominio.** Un perfil comprado o spameado suele estar en 20:1 o 50:1 — cientos de enlaces del mismo sitio. El tuyo es un ratio sano: los enlaces vienen repartidos, que es lo que hace un perfil natural.

## Lo que sí es spam: dos redes, ambas de hace un mes

Analizados los 100 enlaces de peor DR (todos DR 0). **43 marcados como spam por Ahrefs**, y 37 con anchors inequívocos:

### Red 1 — `seo-anomaly-top-N.xyz` (20 dominios)

Veinte dominios numerados secuencialmente: `seo-anomaly-top-161.xyz`, `-162`, `-163`… hasta `-180`. Todos con el mismo texto de ancla:

> `TELEGRAM @SEO_ANOMALY - SEO BACKLINKS, BLACK-LINKS, TRAFFIC BOOST, LINK INDEXING`

Todos apuntan **a la misma página**: `/products/dr-dabber-xs-nano-e-rig-vaporizer-khalifa-kush-edition`. Primer avistamiento: **16 de agosto de 2026**.

**Los 20 son `nofollow`.**

### Red 2 — dominios `.shop` (10 dominios)

`balrio.shop`, `bramo.shop`, `brilko.shop`, `brinto.shop`, `cinvo.shop`, `forvi.shop`, `fralto.shop`, `mervi.shop`, `orvelo.shop`, `plurio.shop` — nombres generados, todos apuntando a la home con:

> `High Quality Dofollow Backlinks DA 50 PA 40 Premium PBN Network Service smokerolla.com Rank First Page Google Fast SEO Link Building Buy Backlinks Online Cheap`

**Estos 10 sí son `dofollow`.**

## Qué es esto realmente

**No lo compró nadie de tu equipo.** El patrón es inconfundible: son **vendedores de servicios SEO usando tu dominio como escaparate**. Publican "smokerolla.com" en sus páginas de demostración para enseñar a clientes potenciales que pueden generar enlaces. Tu marca aparece como muestra de producto, no como beneficiaria.

Se reconoce porque el ancla **describe su servicio**, no tu tienda. Un enlace comprado de verdad diría "dab rigs" o "comprar bongs"; estos dicen "compra backlinks, contacta por Telegram".

## Recomendación: no hacer nada

Va contra el instinto, pero es la postura correcta, y la razona Google:

**1. Google ya los ignora.** Desde 2012 con Penguin 4.0, los enlaces spam se **devalúan**, no penalizan. Google asume que no controlas quién te enlaza — si no fuera así, cualquiera podría hundir a un competidor comprándole enlaces basura.

**2. El volumen es irrelevante.** 30 dominios sobre 564 es el **5%**, todos DR 0 y tráfico 0. Sin peso que transferir, ni bueno ni malo.

**3. Veinte son nofollow.** No pasan señal por definición.

**4. El disavow hace más daño que bien.** Google ha sido explícito: la mayoría de sitios no deberían usarlo nunca. Un disavow mal construido bloquea enlaces buenos por error, y es irreversible en la práctica. John Mueller lo ha repetido: úsalo solo si tienes una **acción manual** en Search Console o compraste enlaces tú mismo.

**Ninguna de esas condiciones se cumple aquí.**

## Cuándo sí actuar

Revisa Search Console → Seguridad y acciones manuales. **Si no hay aviso, no hay nada que arreglar.** Y conviene vigilar si:

- Los dominios `.xyz` pasan de 20 a cientos
- Aparecen anchors de otros sectores (farmacia, casino, adulto) — señal de ataque SEO negativo real
- Llega una acción manual por "enlaces no naturales"

## La pérdida de dominios: eso sí merece atención

Has pasado de **1,743 dominios históricos a 564** — el 68% desaparecido. Esa es la cifra que importa, mucho más que el spam.

Puede ser depuración natural (directorios caducados, sitios muertos) o pérdida de enlaces buenos. **No lo sé todavía** y conviene averiguarlo: recuperar enlaces perdidos suele ser más rentable que construir nuevos, y tu perfil lo necesita — las colecciones tienen mediana de **0 dominios de referencia**.

## Enlaces legítimos encontrados

En la misma muestra, sitios reales del nicho que te enlazan: `hotboxsupplies.com` (anchors "Raw Bamboo Six Shooter", "alien bong"), `weedfanalia.com` ("best hemp wraps", "natural bamboo bongs"), `rodeowholesale.com`. Bajo DR pero temáticamente correctos — el tipo de enlace que sí suma.

Y `architectcommerce.com` con 35 enlaces: un agregador que lista tu catálogo ("smokerolla.com — 3006 products"). Todos nofollow, inofensivo.

← [[smokerolla-dtc-seo/seo-audit]]
