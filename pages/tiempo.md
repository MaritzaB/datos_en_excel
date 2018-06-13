---
layout: page
title: Fecha y hora
description: Formato para guardar fechas y horas
---

Guarda las fechas y horas en Excel como _texto_, no como fecha ni hora. De lo contrario, Excel guardará internamente la fecha como entero y las horas como una fracción. Y cuando importemos los datos no obtendremos lo mismo que tú viste al momento de guardar el archivo.

- Selecciona las celdas con fechas u horas
- Haz clic con el botón derecho
- Selecciona "Formato de Celdas..."
- Selecciona "Texto" del lado izquierdo

En los metadatos usa `axis: T` para las columnas que contengan fechas u horas.

Guarda la fecha en una columna y la hora en otra columna.

Para las fechas usa el formato "`DD/MMM/AAAA`", por ejemplo, "`01/Ene/2018`". La fecha es una cadena de exactamente 11 caracteres de longitud.

En los metadatos usa:
> `standard_name`: `date`
para las columnas que contengan fechas.

Para las horas usa el formato "`hh:mm:ss`", por ejemplo, "`18:00:00`". La hora es una cadena de exactamente 8 caracteres de longitud.

En los metadatos usa:
> `standard_name`: `time`
para las columnas que contengan horas del día.

---

Siguiente: [Validar un archivo de Excel](validacion.html).

(Anterior: [Variables independientes](axis.html).)