---
layout: page
title: Se consistente
description: La regla más importante de la organización de datos es ser consistente
---

La regla más importante de la organización de datos es *ser consistente*.

- **Usa códigos consistentes para las variables categóricas.** Para una variable categórica como *isla* usa siempre un único codigo para referirte a la misma isla, por ejemplo, para las Islas Coronado puedes usar el código "`coronado`". No escribas a veces "`Coronado`" y a veces "`Coronados`" y a veces "`Isla Coronado`" y a veces "`Isla Coronados`" y a veces "`Islas Coronados`". Otro ejemplo son los nombres de las especies. Elije uno y quédate con él.

- **Usa "`NA`" cuando te haga falta un dato.** Ninguna celda en la hoja de datos puede quedar vacía, ni siquiera cuando no tenemos el dato. En GECI usamos "`NA`" (_not available_) para indicar que el dato no está disponible. Además, no insertes una nota en lugar del dato faltante explicando por qué falta. Más bien agrega dicha nota en una columna para notas.

- **Usa nombres de archivos consistentes.** Nombra tus archivos indicando, siempre en el mismo orden, el tipo de monitoreo (o simplemente la palabra Datos), variable(s), especie (o grupo), isla (o región geográfica) y fecha de última actualización. E.g. "`Censo_Nidos_Albatros_Guadalupe_01Ene2018`", "`Busqueda_Madrigueras_AvesMarinas_PacificoNorte_01Ene2018`", etc. Además, no uses espacios, usa guion bajo "`_`".

- **Usa el formato "`DD/MMM/AAAA`" para todas las fechas** Por ejemplo, "`07/Oct/1998`", "`01/Ene/2000`", etc.

- **Ten cuidado con los espacios dentro de las celdas.** Una celda en blanco es diferente de una celda que contiene un solo espacio. Considera que "` macho`" es diferente de "`macho `" (es decir, con espacio al principio o al final). Estas resultarán en una gran frustración y pérdida de tiempo en el mejor de los casos; en el peror de los casos obtendremos resultados incorrectos.

---

&rarr; Siguiente: [Nombres de archivos y columnas](nomenclatura.html).

&larr; Anterior: [Datos](datos.html).
