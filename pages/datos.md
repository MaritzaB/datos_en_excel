---
layout: page
title: Datos
description: Cómo agregar metadatos a un archivo de datos en Excel
---

Guía rápida
-----------

1. Los datos se usan el esquema [_Tidy data_](http://dx.doi.org/10.18637/jss.v059.i10)
1. Los metadatos siguen la [Convención CF](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/build/cf-conventions.html#attribute-appendix) para describir los atributos del conjunto de datos
1. Los datos y metadatos se empaquetan según el formato [_Tabular Data Package_](http://dataprotocols.org/tabular-data-package/)

Datos
-----

Los datos usan el esquema [_Tidy data_](http://dx.doi.org/10.18637/jss.v059.i10). Cada variable es una columna, cada observación es un renglón y cada tipo de unidad observacional es una tabla. Por lo tanto, todos los valores en una misma columna tienen las mismas unidades, mientras que los valores en un mismo renglón pueden tener unidades distintas.

### Ejemplos

Por lo general, una hoja de campo será distinta a la tabla en la que se guardarán los datos. Es común que una tabla en la que se guardan los datos tenga más renglones que la correspondiente hoja de campo.

Por ejemplo, podríamos tener una hoja de campo para el _número de individuos avistados_ de la forma siguiente

Especie   | 2015-06-15 | 2015-06-16 | 2015-06-17
----------|------------|------------|------------
Dragón    |         25 |         41 |         23
Fénix     |        732 |        658 |        874
Unicornio |          1 |          0 |          2

o, tal vez, en una forma alternativa

Fecha      | Dragón | Fénix  | Unicornio
-----------|--------|--------|----------
2015-06-15 |     25 |    732 |        1
2015-06-16 |     41 |    658 |        0
2015-06-17 |     23 |    874 |        2

Las hojas de campo anteriores tienen 4 columnas y 3 renglones con datos;
mientras que la correspondiente tabla en la que se guardan los datos tiene 3 columnas y 9 renglones con datos.

Fecha      | Especie   | Número total de individuos
-----------|-----------|----------------------------
2015-06-15 | Dragón    |  25
2015-06-15 | Fénix     | 732
2015-06-15 | Unicornio |   1
2015-06-16 | Dragón    |  41
2015-06-16 | Fénix     | 658
2015-06-16 | Unicornio |   0
2015-06-17 | Dragón    |  23
2015-06-17 | Fénix     | 874
2015-06-17 | Unicornio |   2

El primer renglón de la tabla de datos debe contener nombres únicos para cada columna.
A veces, la cantidad de unidades es un buen indicador del número de columnas que se debe tener, considerando que todos los datos que resultan de conteos tienen el mismo tipo de unidad.
---

Siguiente: [Se consistente](consistencia.html).

(Anterior: [Introducción](intro.html).)