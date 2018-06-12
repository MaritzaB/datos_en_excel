---
layout: page
title: Metadatos
description: Cómo agregar metadatos a un archivo de datos en Excel
---

Los metadatos proporcionan información adicional sobre los datos. La tabla siguiente muestra la lista de matadatos reconocidos por este protocolo. La columna _Tipo_ indica si el metadato es para toda la tabla o sólo para una columna.

Metadato           | Tipo    | Descripción
-------------------|---------|-------------
`name`             | Tabla   | [The name is a simple name or identifier to be used for this resource](http://specs.frictionlessdata.io/data-resource/#name)
`id`               | Tabla   | Igual que [`name`](http://specs.frictionlessdata.io/data-resource/#name) pero sin ".", "-" ni "_"
`path` o `data`    | Tabla   | [Property describing the location of the data associated to the resource](http://specs.frictionlessdata.io/data-resource/#data-location)
`profile`          | Tabla   | [A string identifying the profile of this descriptor as per the profiles specification](http://specs.frictionlessdata.io/profiles/)
`description`      | Tabla   | [A description of the resource](http://specs.frictionlessdata.io/data-resource/#optional-properties)
`source`           | Tabla   | [The method of production of the original data](http://cfconventions.org/cf-conventions/cf-conventions.html#description-of-file-contents)
`title`            | Tabla   | [A succinct description of what is in the dataset (written in English)](http://www.unidata.ucar.edu/netcdf/docs/netcdf.html#Attribute-Conventions)
`titulo`           | Tabla   | Traducción al español de `title`
`name`             | Columna | [This property should correspond to the name of field/column in the data file](http://specs.frictionlessdata.io/table-schema/#name)
`axis`             | Columna | [Identifies latitude, longitude, vertical, or time axes](http://cfconventions.org/cf-conventions/cf-conventions.html#coordinate-types)
`description`      | Columna | [A description for this field](http://specs.frictionlessdata.io/table-schema/#description)
`long_name`        | Columna | [A descriptive name that indicates a variable's content (written in English). This name is not standardized ](http://cfconventions.org/cf-conventions/cf-conventions.html#long-name)
`nombre_largo`     | Columna | Traducción al espanol de `long_name`
`standard_name`    | Columna | [A standard name that references a description of a variable's content in the standard name table](http://cfconventions.org/standard-names.html)
`units`            | Columna | [Units of a variable's content](http://www.unidata.ucar.edu/software/udunits/udunits.txt)

---

Siguiente: [Nombre estándar](pages/standard_name.html).

(Anterior: [Datos](pages/datos.html).)