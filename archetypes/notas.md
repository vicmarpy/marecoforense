---
title: "{{ replace .File.ContentBaseName "-" " " | humanize }}"
date: {{ .Date }}
# Cambiar a false (o borrar la línea) para publicar la nota.
draft: true
# Una o dos frases. Aparece en el listado de notas y en los buscadores.
description: ""
tags: []
---

## Resumen

_Dos o tres frases: qué problema aborda esta nota y qué conclusión deja._

## Contexto

_Situación, tipo de caso o pregunta de partida. Sin datos de casos reales ni de personas._

## Procedimiento o análisis

_Pasos técnicos, herramientas usadas y por qué. Cada paso en un párrafo corto o en una lista numerada._

## Hallazgos

_Qué se observó y qué significa._

## Recomendaciones prácticas

_Qué hacer y qué evitar, en lenguaje que entienda un abogado o un responsable de TI._

## Referencias

_Normas, documentación de herramientas, estándares (por ejemplo, ISO/IEC 27037) o artículos consultados._
