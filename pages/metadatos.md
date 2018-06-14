---
layout: page
title: Metadatos
description: Cómo agregar metadatos a un archivo de datos en Excel
---

- Los metadatos de una tabla de datos se guardan en la segunda hoja de un archivo de Excel.
- Cada renglón representa una variable y cada columna representa un conjunto de metadatos.
- La primer columna se usa para indicar el nombre de las variables.
- El primer renglón contiene los nombres de los metadatos.
- Un renglón contiene los valores de los metadatos de la tabla completa.
- En el resto de los renglones contienen los valores de los metadatos de cada variable.
- La cantidad de renglones en la hoja de metadatos es igual a la suma de la cantidad de columnas de la hoja de datos más dos.
- Es indispensable incluir en los metadatos de las variables el `long_name` y `nombre_largo` y en los metadatos globales el `title` y `titulo`.

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

Siguiente: [Nombre estándar](standard_name.html).

(Anterior: [Ninguna celda vacía](ninguna_celda_vacia.html).)
