---
layout: page
title: Fecha y hora
description: Formato para guardar fechas y horas
---

Guarda las fechas y horas en Excel como _texto_, no como fecha ni hora. De lo contrario, Excel guardará internamente las fechas como entero y las horas como fracciones. Y cuando importemos los datos no obtendremos lo mismo que tú viste al momento de guardar el archivo.

En Excel:

- Selecciona las celdas con fechas u horas
- Haz clic con el botón derecho
- Selecciona "Formato de Celdas..."
- Selecciona "Texto" del lado izquierdo

Guarda la fecha en una columna y la hora en otra columna distinta. Usa "`axis: T`" en los metadatos de las columnas que contengan fechas u horas.

Para las fechas usa el formato "`DD/MMM/AAAA`", por ejemplo, "`01/Ene/2018`". La fecha es una cadena de exactamente 11 caracteres de longitud. En los metadatos usa "`standard_name`: `date`".

Para las horas usa el formato "`hh:mm:ss`", por ejemplo, "`18:00:00`". La hora es una cadena de exactamente 8 caracteres de longitud. En los metadatos usa "`standard_name`: `time`".

---

&rarr; Siguiente: [Validar un archivo de Excel](validacion.html).

&larr; Anterior: [Coordenadas UTM](utm.html).