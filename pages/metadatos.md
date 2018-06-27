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

_Tabla: Ejemplo de tabla de metadatos_

**name**   | **nombre_largo** | **long_name** | **standard_name** | **axis** | **units**     | **titulo**                                             | **title**
-----------|------------------|---------------|-------------------|----------|---------------|--------------------------------------------------------|------------------------------------
**TABLA**  | NA               | NA            | NA                | NA       | NA            | Muestreo por cuadrantes de madrigueras de aves marinas | Quadrat sampling of seabird burrows
**lat**    | Latitud          | Latitude      | latitude          | Y        | degree_north  | NA                                                     | NA
**lon**    | Longitud         | Longitude     | longitude         | X        | degree_west   | NA                                                     | NA
**conteo** | Madrigueras      | Burrows       | NA                | NA       | NA            | NA                                                     | NA

En el ejemplo anterior, el nombre de la tabla de datos es **TABLA** y el título de la tabla es "_Muestreo por cuadrantes de madrigueras de aves marinas_". Además, la tabla de datos tiene tres columnas **lat**, **lon** y **conteo**. ([Aquí](resumen.html) puedes ver la tabla de datos correspondiente.) También se aprecia en el ejemplo anterior que [ninguna celda está vacía](celdas_vacias.html); se indica con "NA" que "_no aplica_" o que no se cuenta con el valor faltante.

En la tabla de metadatos el primer renglón muestra el nombre de los metadatos, el segundo renglón contiene los metadatos de la tabla de datos completa, y el resto de los renglones contienen los metadatos de cada columna de datos. La primer columna en la tabla de metadatos contiene el nombre de la tabla de datos y de sus columnas.

La información que nos proporcionan los metadatos nos ayudan a visualizar y procesar los datos. Por ejemplo, **nombre_largo** podría ser la etiqueta que usemos en los ejes de alguna gráfica. También podríamos transformar unidades de forma automática si incluímos el metadato **units**. Podríamos convertir de [coordenadas geográfica](pages/geograficas.html) a [coordenadas UTM](pages/utm.html) o viceversa al incluir los metadatos [**axis**](axis.html) y [**standard_name**](standard_name.html) correspondientes.

### Tipos de Metadatos

Hay dos tipos de metadatos: los _metadatos de la tabla_ que describen la tabla de datos en general, y los _metadatos de columna_ que describen cada columna de datos en particular. La tabla siguiente muestra la lista de metadatos de este protocolo y para cada metadato indica si es de tabla o de columna.

_Tabla: Matadatos reconocidos por este protocolo. La primer columna indica el nombre del metadato; la segunda columna indica si el metadato es para toda la tabla o sólo para una columna; la última columna describe al metadato._

Metadato           | Tipo    | Descripción
-------------------|---------|-------------
`name`             | Tabla   | [Nombre o identificador de esta tabla](http://specs.frictionlessdata.io/data-resource/#name)
`id`               | Tabla   | Igual que [`name`](http://specs.frictionlessdata.io/data-resource/#name) pero sin ".", "-" ni "_"
`description`      | Tabla   | [Descripción detallada de la tabla. Generalmente más larga que `titulo` y `title`](http://specs.frictionlessdata.io/data-resource/#optional-properties)
`source`           | Tabla   | [Fuente de los datos originales](http://cfconventions.org/cf-conventions/cf-conventions.html#description-of-file-contents)
`title`            | Tabla   | [Titulo de la tabla en inglés para ser usada como encabezado dentro de un reporte. Generalmente más breve que `description`](http://www.unidata.ucar.edu/netcdf/docs/netcdf.html#Attribute-Conventions)
`titulo`           | Tabla   | Traducción al español de `title`
`name`             | Columna | [Noombre de la columna en la hoja de datos](http://specs.frictionlessdata.io/table-schema/#name)
`axis`             | Columna | [Identifica coordenadas o tiempo con las letras `X`, `Y`, `Z` o `T`](axis.html)
`description`      | Columna | [Descripción de la columna de datos](http://specs.frictionlessdata.io/table-schema/#description)
`long_name`        | Columna | [Nombre descriptivo de la columna en inglés para ser usado como rótulo en los ejes de las gráficas](http://cfconventions.org/cf-conventions/cf-conventions.html#long-name)
`nombre_largo`     | Columna | Traducción al espanol de `long_name`
`standard_name`    | Columna | [Nombre estándar de la variable](standard_name.html)
`units`            | Columna | [Unidades de los valores de la columna de datos](units.html)

No es necesario que te limites a los metadatos enlistados en la tabla anterior. Puedes agregar cualquier metadato que te ayude a comunicar la historia detallada detrás de los datos.

---

&rarr; Siguiente: [Nombre estándar](standard_name.html).

&larr; Anterior: [No uses colores en lugar de datos](sin_colores.md).
