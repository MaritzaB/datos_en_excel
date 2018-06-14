---
layout: page
title: Resumen
description: datos en excel
---

- Los datos de una actividad de monitoreo se guardan en una o varias tablas de datos.
- Cada tabla de datos se guarda en un archivo de Excel distinto, es decir, cada archivo de Excel contiene una única tabla de datos.
- Cada archivo de Excel debe tener dos hojas: la primera para los datos y la segunda para los metadatos.
- En la hoja de datos, cada columna representa una variable y cada renglón representa una observación.
- En la hoja de los datos, el primer renglón se usa para indicar el nombre de las variables.
- En la hoja de los metadatos, cada renglón representa una variable y cada columna representa un conjunto de metadatos.
- En la hoja de los metadatos, la primer columna se usa para indicar el nombre de las variables.
- En la hoja de los metadatos, el primer renglón contiene los nombres de los metadatos.
- Un renglón contiene los valores de los metadatos de la tabla completa.
- En el resto de los renglones contienen los valores de los metadatos de cada variable.
- La cantidad de renglones en la hoja de metadatos es igual a la suma de la cantidad de columnas de la hoja de datos más dos.
- Es indispensable incluir en los metadatos de las variables el `long_name` y `nombre_largo` y en los metadatos globales el `title` y `titulo`.

---

Siguiente: [Datos](datos.html).

(Inicio: [Contenido](../index.html).)
