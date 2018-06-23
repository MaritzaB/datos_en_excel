---
layout: page
title: Nombres de archivos y columnas
description: Reglas de nomenclatura
---

Es importante nombrar las cosas correctamente, pero es difícil. Vale la pena invertir tiempo y esfuerzo en escoger buenos nombres.

Al nombrar archivos o columnas:

- Solo puedes usar letras (excepto eñe, vocales con acentos y diéresis), números (siempre y cuando el nombre no empiece con número) y guiones bajos (`_`).
- No uses espacios. Puedes usar guiones bajos (`_`). Además, ten cuidado que no haya espacios al final del nombre, por ejemplo, "`envergadura`" es distinto a "`envergadura `".
- No uses símbolos. No uses `$`, `@`, `%`, `#`, `&`, `+`, `*`, `^`, `/`, `(`, `)`, `!`, `°`, `=`, `~`, etcétera. Tampoco uses eñes (`ñ`), vocales con acento (`á`, `é`, `í`, `ó`, `ú`) o diéresis (`ü`).
- No uses abreviaturas. Los nombres deben ser descriptivos, específicos y sin ambigüedades. Por ejemplo, para la variable *temperatura* no uses `Temp`.

Aquí hay una tabla con ejemplos buenos y malos:

**buen nombre**       | **buena alternativa**         | **evita**
--------------------- | ----------------------------- | ---------
`temperatura`         | `Temperatura_C`               | `Temp (°C)`
`precipitacion`       | `Precipitacion_mm`            | `Precipitación`
`productividad`       | `Productividad_PollosPorNido` | `Prod. pollos/nido`
`sexo`                | `Sexo`                        | `Macho/Hembra`
`peso`                | `Peso`                        | `p.`
`tipo_de_rastro`      | `TipoDeRastro`                | `Tipo de rastro`
`primer_huevo`        | `Huevo1`                      | `1er huevo`

---

&rarr; Siguiente: [Ninguna celda vacía](ninguna_celda_vacia.html).

&larr; Anterior: [Se consistente](consistencia.html)
