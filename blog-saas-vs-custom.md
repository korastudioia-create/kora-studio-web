---
title: "SaaS de facturación o app a medida: cuándo gana cada uno (caso real 2026)"
description: "Un cliente pagaba 400€/mes en SaaS. Le montamos una app a medida por 600€ únicos. Cuándo tiene sentido cada opción, sin humo."
pubDate: 2026-04-24
author: "Adrián Burgos"
slug: "saas-facturacion-vs-app-a-medida"
tags: ["facturación", "saas-vs-custom", "pymes", "caso-real"]
metaTitle: "SaaS de facturación vs app a medida: cuándo gana cada uno"
metaDescription: "400€/mes en SaaS o 600€ una vez en app a medida: caso real 2026 de una PYME fotovoltaica. Framework honesto para decidir sin caer en sobreventa."
keywords: ["software facturación a medida", "alternativa a Holded pymes", "desarrollo a medida vs SaaS España"]
---

# SaaS de facturación o app a medida: cuándo gana cada uno (caso real 2026)

400€ al mes, año tras año, por un software que usabas al 20%. O 600€ una sola vez por una aplicación que hace exactamente lo que necesitas. Suena tramposo puesto así, y lo es un poco: las dos opciones tienen su momento. Pero la semana pasada resolvimos este dilema con un cliente del sector fotovoltaico en Sevilla, y el resultado fue lo bastante claro como para escribirlo.

La pregunta no es "¿SaaS o a medida?". La pregunta es **¿en qué punto deja de tener sentido alquilar software genérico y empieza a compensar tener el tuyo?**. Spoiler: depende de tres cosas, y ninguna es el precio del primer mes.

## Los tres costes ocultos del SaaS genérico

Cuando hablamos de SaaS de facturación tipo Holded, FacturaDirecta, Sage, Quipu o similares, el precio de portada nunca es el precio real. Hay tres fugas que casi nadie suma hasta que lleva dos años dentro.

**1. Funcionalidades que pagas y no usas.** Un plan medio de Holded trae CRM, inventario, proyectos, RRHH light, contabilidad… Si tu empresa solo necesita facturar y tener un registro de clientes, estás pagando un 70% de músculo muerto. Y no, no hay un "plan solo facturación" serio: los planes bajos suelen capar número de facturas o usuarios.

**2. Módulos que escalan al alza.** Empiezas en 29€/mes, añades multi-usuario (+15€), conciliación bancaria (+20€), TPV (+25€), y en seis meses estás en 150-200€ sin haberte enterado. Sumado a un segundo SaaS complementario (tipo Stripe, Factorial o un CRM), pasas los 300-400€/mes fácil.

**3. Dependencia.** Tus datos viven en su base de datos, en su formato, con su API. El día que quieras cambiar, migras a pulmón o pagas a alguien para que migre. Y si suben precios un 20% (ha pasado, pasará), tu margen de negociación es cero.

Ninguno de estos costes sale en el primer presupuesto. Los descubres en el mes 14.

## Cuándo el SaaS sigue ganando (y es honesto reconocerlo)

No vendemos desarrollo a medida a todo el mundo. Hay casos donde montar algo propio es una mala decisión y te lo decimos:

- **Eres emisor oficial de facturas y te aplica Verifactu.** La ley 11/2021 y el RD 1007/2023 exigen que el software que emite facturas cumpla requisitos técnicos muy concretos (trazabilidad, firma, envío a la AEAT). Holded, FacturaDirecta y compañía ya están homologados. Montar eso desde cero es carísimo y absurdo si ya existe.
- **Tu equipo no es técnico y necesita soporte 24/7.** Un SaaS grande tiene chat, tutoriales, comunidad. Una app a medida depende de quien te la hizo.
- **Necesitas muchísimas integraciones estándar** (bancos, Amazon, Shopify, pasarelas de pago, gestorías). Reinventar conectores es tirar dinero.
- **Tu proceso cambia cada trimestre.** Si aún no sabes qué necesitas, no paralices la decisión en código. Alquila flexibilidad.
- **Facturas muchísimo y quieres cumplimiento fiscal blindado sin pensar.** Paga y duerme tranquilo.

Si estás en cualquiera de estos cinco supuestos, cierra esta pestaña y quédate con tu SaaS. En serio.

## Cuándo una app a medida gana

Ahora la otra cara. Una app propia empieza a compensar cuando se cumplen varias de estas condiciones a la vez:

- Usas un SaaS pero **solo tocas el 15-25% de sus funciones**.
- Tu necesidad es **un registro interno, no emisión oficial** (lo explicamos más abajo, es crítico).
- El **proceso es estable**: llevas años haciéndolo igual y va a seguir igual.
- Tienes **un flujo único** que ningún SaaS cubre del todo y acabas con Excel al lado.
- Piensas usarlo **más de 24 meses** (el punto de equilibrio casi siempre está ahí).
- Valoras tener **tus datos en tu infraestructura**, exportables, sin candados.

Cuando marcas cuatro de esas seis casillas, la cuenta sale.

## El caso real: sector fotovoltaico, Sevilla, abril 2026

Cliente referido. Empresa mediana del sector fotovoltaico en el sur, equipo de oficina pequeño, gestoría externa que se encarga de la parte fiscal pesada. Vienen con un dolor muy concreto:

> "Llevamos clientes y facturas en un Excel compartido. Se nos está yendo de las manos. Estamos mirando Holded o FacturaDirecta con todos los módulos, nos sale sobre 200-400€/mes. ¿Qué opináis?"

Les hicimos la pregunta clave: **¿emitís vosotros las facturas oficiales o las emite la gestoría?**. Las emite la gestoría. Lo que ellos necesitaban era **un registro interno** para tener controlado quién es cliente, qué se le ha facturado, buscar por DNI, filtrar por trimestre y poder descargar el PDF de una factura rápido sin abrir cinco carpetas.

Con ese alcance, un SaaS fiscal completo era matar moscas a cañonazos. Les montamos en un día una aplicación web con:

- Registro de clientes (alta, búsqueda por DNI/CIF, histórico).
- Catálogo de productos y servicios.
- Generación de facturas con numeración correlativa automática.
- Filtro por trimestre, cliente y producto.
- Descarga de cada factura en PDF.
- Acceso desde navegador, sin instalar nada.

**Stack**, explicado en cristiano: Next.js (un framework moderno para apps web rápidas), Supabase (una base de datos en la nube gestionada) y react-pdf (una librería para generar PDFs bonitos). Todo alojado en infraestructura estándar, sin servidores propios que mantener.

**Cifras:**

| Opción | Coste año 1 | Coste año 2 | Coste 3 años |
|---|---|---|---|
| SaaS estimado (300€/mes) | 3.600€ | 3.600€ | 10.800€ |
| App a medida (Kora Studio) | 840€ | 240€ | 1.320€ |

Ahorro proyectado a tres años: **~9.500€**. Y lo más importante: el software hace exactamente lo que necesitan, ni una función de más, ni una de menos.

## Framework de decisión en 4 preguntas

Antes de firmar un SaaS o de encargar una app, respóndete esto con honestidad:

1. **¿Quién emite tus facturas oficiales?** Si las emite tu gestoría o un sistema ya homologado, lo que tú necesitas es probablemente un registro interno, no un emisor.
2. **¿Qué porcentaje del SaaS usas realmente?** Si es menos del 30%, estás subvencionando funciones ajenas.
3. **¿Tu proceso va a cambiar mucho en los próximos dos años?** Si sí, alquila. Si no, compra.
4. **¿Cuánto pagarías en 24 meses?** Multiplica tu cuota mensual por 24. Compáralo con un desarrollo a medida one-off + mantenimiento. Si el SaaS supera en 2x al custom, la decisión es obvia.

Si tres de las cuatro respuestas apuntan hacia custom, merece la pena al menos pedir presupuesto.

## Aviso legal importante: Verifactu no es opcional si emites facturas

Aquí nos ponemos serios un momento, porque hemos visto a gente confundirlo.

La **Ley 11/2021** (antifraude) y el **Real Decreto 1007/2023** regulan los sistemas informáticos de facturación en España. Si tu empresa emite facturas con software, ese software **debe cumplir los requisitos Verifactu** a partir de las fechas de entrada en vigor que marca la AEAT (julio 2025 para sociedades, enero 2026 para autónomos, con matices por tamaño y obligatoriedad efectiva según Hacienda).

Un **registro interno** —como el que montamos para el cliente fotovoltaico— **no emite facturas oficiales**. Es una herramienta de gestión, como un Excel mejorado. Las facturas oficiales siguen saliendo de la gestoría con su software homologado. Esto es perfectamente legal y es el escenario real de muchísimas PYMEs españolas.

Si tu caso es que **tú sí emites facturas oficiales desde dentro**, entonces o vas a SaaS homologado o encargas un desarrollo a medida que cumpla Verifactu (más caro, con más validaciones, y tiene sentido solo a partir de cierto volumen). No mezcles las dos cosas.

Consulta siempre con tu asesor fiscal antes de decidir. Esto no es asesoramiento legal.

## Conclusión

El SaaS no es el enemigo. Lo es pagar 3.600€ al año por algo que cubre el 20% de lo que tu negocio realmente necesita, cuando por 600€ únicos puedes tener exactamente lo tuyo. La decisión correcta depende de tu caso, no de la moda.

En Kora Studio no vendemos desarrollo a medida a todo el que llama. Si tu situación encaja mejor con un SaaS, te lo decimos y seguimos tan amigos. Si encaja con algo propio, lo montamos sin módulos inflados.

Si tienes dudas de en qué lado estás, te hacemos un **diagnóstico gratuito de 30 minutos**: miramos qué SaaS pagas, qué usas de verdad, y te damos una recomendación honesta. Sin compromiso y sin guion de ventas.
