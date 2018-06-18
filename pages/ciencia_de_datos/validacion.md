---
layout: page
title: Validar un archivo de Excel
tagline: para analistas de datos
description: Cómo verificar si un archivo de Excel cumple con este protocolo

---

Usamos [jsonschema](https://github.com/Julian/jsonschema) para validar que:

- el [descriptor del TDP](https://frictionlessdata.io/specs/tabular-data-package/) generado a partir del segundo renglón de la segunda hoja de Excel (el primer renglón es el encabezado) cumple con [este JSON Schema](https://frictionlessdata.io/schemas/tabular-data-package.json),
- el [descriptor del recurso de datos tabulados](http://frictionlessdata.io/specs/tabular-data-resource/) (generado a partir del resto de la segunda hoja de Excel) cumple con [este JSON Schema](http://frictionlessdata.io/schemas/tabular-data-resource.json), y
- el [esquema de la tabla](http://frictionlessdata.io/specs/table-schema/) (especificado por el [descriptor del recurso de datos tabulados](http://frictionlessdata.io/specs/tabular-data-resource/)) cumple con [este JSON Schema](http://frictionlessdata.io/schemas/table-schema.json).

Usamos [_Good Tables_](https://goodtables.readthedocs.io) para validar que la tabla de datos CSV (generada a partir de la primer hoja del archivo de Excel) cumple con el [esquema de la tabla](http://frictionlessdata.io/specs/table-schema/) (especificado por el [descriptor del recurso de datos tabulados](http://frictionlessdata.io/specs/tabular-data-resource/))

---

Inicio: [Información adicional para analistas de datos](index.html)
