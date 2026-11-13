---
title: "Cómo preservar un correo electrónico como prueba"
date: 2026-10-15
description: "Qué hacer para conservar un correo electrónico de forma que pueda verificarse su origen y contenido: por qué no alcanza con imprimirlo o reenviarlo."
draft: false
---

Un correo electrónico puede ser prueba de un acuerdo, de una intimación, de una instrucción laboral o de una oferta comercial. Pero un correo impreso o reenviado a otra persona pierde justamente lo que permitiría verificarlo. Esta guía explica cómo conservarlo correctamente.

## Qué contiene realmente un correo

Lo que se ve en pantalla (remitente, asunto, fecha y texto) es solo una parte. Cada mensaje lleva además un conjunto de datos técnicos llamados **encabezados**, que registran el recorrido del correo entre servidores, los identificadores del mensaje y los resultados de las verificaciones de autenticidad del remitente (como SPF, DKIM y DMARC).

Esos encabezados son los que permiten, en una pericia, evaluar si el mensaje realmente salió del dominio que dice haber salido y si fue alterado en el camino.

## Lo primero: no borrar ni mover nada

- Conservar el mensaje en la cuenta donde se recibió, sin eliminarlo ni vaciar la papelera.
- No cerrar ni dar de baja la cuenta mientras el asunto esté abierto.
- Si el correo está en una computadora de trabajo, avisar antes de que se reasigne o se formatee el equipo.

## Por qué no alcanza con imprimir o reenviar

- **Imprimir o sacar una captura** deja solo la apariencia del mensaje, sin los encabezados.
- **Reenviar** crea un mensaje nuevo: cambia el remitente, la fecha y el contenido técnico. Lo que recibe el destinatario ya no es el original.
- **Copiar y pegar el texto** en otro documento elimina toda la información técnica.

Estas copias pueden servir como referencia, pero no reemplazan el mensaje original.

## Cómo conservar el mensaje original

La mayoría de los servicios permite descargar el mensaje completo como un archivo, normalmente con extensión `.eml` o `.msg`. Por ejemplo, Gmail ofrece la opción "Descargar mensaje" y también "Mostrar original", que permite ver los encabezados. Outlook y los clientes de escritorio permiten guardar el mensaje como archivo.

Conviene:

1. Descargar el mensaje original, junto con sus adjuntos, sin abrirlos para editarlos.
2. Guardar el archivo en un lugar seguro, sin renombrarlo ni modificarlo.
3. Calcular su hash en ese momento (véase la nota sobre el hash), para poder demostrar después que no cambió.
4. Conservar también el hilo completo de la conversación, no solo el mensaje que parece más importante.

## Cuando el correo es de la empresa

Si el correo está en un servidor corporativo o en una cuenta que el titular no controla, no debe intentarse acceder por cuenta propia. La obtención debe hacerla quien tiene autoridad sobre el sistema, de manera documentada, para que la evidencia no pueda cuestionarse por su forma de obtención.

## Un cuidado importante

Acceder a la cuenta de otra persona sin autorización puede constituir un delito y además invalidar la prueba. Si el correo está en una cuenta ajena, lo adecuado es consultar primero sobre el camino correcto.

## ¿Necesita preservar correos para un caso?

Si el mensaje puede ser importante, conviene preservarlo antes de seguir usando la cuenta. Puede escribirme desde la página de [Contacto](/contacto/).
