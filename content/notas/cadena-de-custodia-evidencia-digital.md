---
title: "Cadena de custodia de la evidencia digital: qué es y por qué importa"
date: 2026-10-14
# Nota de ejemplo. Está como borrador: no se publica hasta cambiar a false.
draft: true
description: "Una evidencia digital solo sirve si se puede demostrar que no cambió desde que se obtuvo. Eso es lo que documenta la cadena de custodia."
tags: ["evidencia digital", "cadena de custodia"]
---

## Resumen

La evidencia digital se copia, se altera y se borra con mucha facilidad. Por eso no alcanza con tener el archivo: hay que poder demostrar quién lo obtuvo, cuándo, cómo y que no se modificó. La cadena de custodia es el registro que lo respalda.

## Qué se documenta

Una cadena de custodia ordenada deja constancia de:

1. Qué dispositivo o dato se recibió, con su descripción y estado (marca, modelo, número de serie, si estaba encendido o apagado).
2. Quién lo entregó, quién lo recibió y en qué fecha y hora.
3. Dónde y cómo se almacenó entre una intervención y otra.
4. Qué procedimientos se aplicaron y con qué herramientas.

## El rol del hash

Al crear una copia forense se calcula un valor hash (por ejemplo, SHA-256) del original y de la copia. Si ambos coinciden, la copia es idéntica bit a bit. Cualquier cambio posterior, aunque sea de un solo byte, produce un hash distinto.

```
sha256sum imagen_disco.dd
```

El valor obtenido se anota en el acta y en el informe, para que otro perito pueda repetir la verificación.

## Recomendaciones prácticas

- No encender, navegar ni "revisar" un dispositivo que puede ser evidencia: cada uso lo modifica.
- No reenviar ni reenviarse archivos por mensajería como si fueran la evidencia original.
- Consultar a un perito antes de intervenir, no después.

## Referencias

- ISO/IEC 27037: directrices para la identificación, recolección, adquisición y preservación de evidencia digital.
