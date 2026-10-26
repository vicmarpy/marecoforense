---
title: "Qué es el hash y por qué importa en una pericia"
date: 2026-10-26
description: "El hash es la huella digital de un archivo. Explica cómo se usa para demostrar que una evidencia digital no fue alterada y cuáles son sus límites."
draft: false
---

En una pericia informática se habla mucho de "hash", y con razón: es una de las herramientas que permiten demostrar que una evidencia digital no cambió desde que se obtuvo. Este artículo explica qué es, para qué sirve y qué no puede probar.

## Qué es un hash

Un hash es una huella digital de un archivo o de un disco completo. Un algoritmo matemático lee todo el contenido y produce una cadena corta de letras y números, por ejemplo de 64 caracteres en el caso de SHA-256.

Tiene tres propiedades que lo hacen útil:

- **El mismo contenido siempre produce el mismo hash.**
- **Cualquier cambio, por mínimo que sea, produce un hash totalmente distinto.** Basta con modificar una coma o un solo píxel.
- **No se puede reconstruir el archivo a partir del hash.** Es una huella, no una copia.

## Para qué se usa en una pericia

Al adquirir una evidencia, el perito calcula el hash de la fuente original y el de la copia forense. Si coinciden, la copia es idéntica a la original. Después, cada vez que se vuelve a calcular el hash de la copia, un resultado igual demuestra que no fue modificada.

Por eso el hash es una pieza central de la **cadena de custodia**: deja constancia, con un dato verificable, de que el material analizado es el mismo que se obtuvo al principio. El informe pericial suele incluir los valores de hash de cada elemento relevante.

## Un ejemplo práctico

Si usted conserva un archivo importante (un video, un contrato en PDF, la exportación de un chat), puede calcular su hash en el momento en que lo recibe y anotarlo. Si más adelante alguien cuestiona que el archivo fue alterado, volver a calcular el hash permite comprobarlo.

En una computadora Mac, desde la Terminal:

```
shasum -a 256 nombre-del-archivo
```

En Windows, desde el Símbolo del sistema:

```
certutil -hashfile nombre-del-archivo SHA256
```

Para un caso importante, lo recomendable es que este paso lo documente un perito, porque la fecha y el procedimiento también cuentan.

## Qué no demuestra el hash

El hash prueba **integridad**: que el archivo no cambió desde que se calculó. No prueba que el contenido sea verdadero ni que haya sido auténtico desde el principio. Si un archivo ya estaba manipulado cuando se calculó su hash, el hash solo confirma que sigue igual de manipulado.

Por eso la pericia no se limita a calcular el hash: analiza el origen del archivo, sus metadatos y el contexto en que se obtuvo.

## Algoritmos: MD5, SHA-1 y SHA-256

Existen varios algoritmos. MD5 y SHA-1 se usaron durante años, pero hoy se consideran débiles frente a ataques que buscan fabricar dos archivos distintos con el mismo hash. En la práctica pericial actual se prefiere SHA-256, y a veces se calculan varios algoritmos a la vez.

## ¿Necesita asegurar una evidencia?

Si tiene archivos que pueden ser importantes en un caso, lo mejor es preservarlos antes de modificarlos o reenviarlos. Puede consultarme desde la página de [Contacto](/contacto/).
