---
layout: page
title: Introducción
description: Presentación para los biólogos del protocolo para guardar datos en Excel
---

Implementación en diferentes formatos
-------------------------------------

En esta sección se describe como se implementa esta guía en los diferentes formatos usados por el grupo.

### Tabular Data Package

[Tabular Data Package](http://dataprotocols.org/tabular-data-package/) (TDP) es el formato preferido por esta guía. En este formato cada actividad de monitoreo constituye un directorio. Los datos se guardan en un archivo CSV y los metadatos correspondientes en un archivo JSON.

### Excel

En Excel cada actividad de monitoreo constituye un archivo. Cada archivo de Excel debe tener dos hojas: la primera para los datos y la segunda para los metadatos. El resto de las hojas del archivo de Excel son para uso discrecional; no interfieren en el procesamiento de datos.

#### Datos en Excel

En la hoja de datos, cada columna representa una variable y cada renglón representa una observación. El primer renglón se usa para indicar el nombre de las variables.

#### Metadatos en Excel

En la hoja de los metadatos, cada columna representa un atributo y cada renglón representa una variable. La primer columna se usa para indicar el nombre de las variables.

El primer renglón de la tabla contiene los nombres de los atributos. En el resto de los renglones se encuentran los valores de los atributos. Uno de los renglones contiene los valores de los atributos globales.

La hoja de metadatos siempre tiene dos renglones más que el número de columnas de la hoja de datos.

Es indispensable incluir en los atributos de las variables el `long_name` y `nombre_largo` y en los atributos globales el `title` y `titulo`.

---

Siguiente: [Datos](datos.html).

(Inicio: [datos en excel](../index.html).)