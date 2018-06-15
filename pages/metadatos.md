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

---

**Los metadatos te dan cierto control sobre el aspecto que tienen las gráficas que el equipo de Ciencia de Datos genera para ti.** Los metadatos nos proporcionan información adicional sobre los datos, como: unidades, nombres en diferentes idiomas, nombre de la persona que colectó los datos, método usado para la colecta de datos, instrumento de medición, referencias, etcétera.

Cada archivo de datos en Excel debe tener en su segunda hoja una tabla con los metadatos. (En la primer hoja se guarda la tabla de datos.) Aquí hay un ejemplo de una tabla de metadatos.

_Tabla: Ejemplo de hoja de metadatos_

**name**   | **nombre_largo** | **long_name** | **standard_name** | **axis** | **titulo**                                             | **title**
-----------|------------------|---------------|-------------------|----------|--------------------------------------------------------|------------------------------------
**TABLA**  | NA               | NA            | NA                | NA       | Muestreo por cuadrantes de madrigueras de aves marinas | Quadrat sampling of seabird burrows
**lat**    | Latitud          | Latitude      | latitude          | Y        | NA                                                     | NA
**lon**    | Longitud         | Longitude     | longitude         | X        | NA                                                     | NA
**conteo** | Madrigueras      | Burrows       | NA                | NA       | NA                                                     | NA

En la tabla de metadatos el primer renglón muestra el nombre de los metadatos, el segundo renglón contiene los metadatos de la tabla de datos completa, y el resto de los renglones contienen los metadatos de cada columna de datos. La primer columna en la tabla de metadatos contiene el nombre de la tabla de datos y de sus columnas.

En el ejemplo anterior, el nombre de la tabla de datos es **TABLA** y el título de la tabla es "_Muestreo por cuadrantes de madrigueras de aves marinas_". Además, la tabla de datos tiene tres columnas **lat**, **lon** y **conteo**. En la tabla de metadatos [ninguna celda está vacía](ninguna_celda_vacia.html).

La información que nos proporcionan los metadatos nos ayudan a visualizar y procesar los datos. Por ejemplo, **nombre_largo** podría ser la etiqueta que usemos en los ejes de alguna gráfica. También podríamos transformar unidades de forma automática si incluímos el metadato **units**. Podríamos convertor de [coordenadas geográfica](pages/geograficas.html) a [coordenadas UTM](pages/utm.html) o viceversa al incluir los metadatos [**axis**](axis.html) y [**standard_name**](standard_name.html) correspondientes.

### Tipos de Metadatos

Hay dos tipos de metadatos: los _metadatos de la tabla_ que describen la tabla de datos en general, y los _metadatos de columna_ que describen cada columna de datos en particular. La tabla siguiente muestra la lista de metadatos de este protocolo y para cada metadato indica si es de tabla o de columna.

_Tabla: Matadatos reconocidos por este protocolo. La primer columna indica el nombre del metadato; la segunda columna indica si el metadato es para toda la tabla o sólo para una columna; la última columna describe al metadato._

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

No es necesario que te limites a los metadatos enlistados en la tabla anterior. Puedes agregar cualquier metadato que te ayude a comunicar la historia detallada detrás de los datos.

---

Siguiente: [Nombre estándar](standard_name.html).

(Anterior: [Ninguna celda vacía](ninguna_celda_vacia.html).)
