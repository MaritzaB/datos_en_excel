---
layout: page
title: Se consistente
description: La primera regla de la organización de datos
---

La primera regla de la organización de datos es *ser consistente*.

- **Usa códigos consistentes para variables categóricas.** Para una variable categórica como *sexo*, usa un único valor común para machos (por ejemplo, `macho`) y un único valor común para las hembras (por ejemplo, `hembra`). No escribas a veces `M` , a veces `macho`, y a veces `Macho`. Elije uno y quédate con él.

- **Usa `NA` cuando te haga falta un dato.** Ninguna celda en la hoja de datos puede quedar vacía, ni siquiera cuando no tenemos el dato. En GECI usamos `NA` (_not available_) para indicar que el dato no está disponible.
Además, no insertes una nota en lugar del dato faltante explicando por qué falta. Más bien agrega dicha nota en una columna para notas.

- **Usa IDs consistentes.** Si a veces es `153` y a veces `raton153` y a veces `ratón153` y a veces `raton-153F` y a veces `Raton153`, vamos a tener que trabajar extra para descubrir quién es quien.

- **Usa un diseño de datos común en archivos múltiples.** Si tus datos están en varios archivos, usa el mismo diseño en todos los archivos.

- **Usa nombres de archivos consistentes.** Nombra tus archivos indicando siempre en el mismo orden tipo de monitoreo (o simplemente la palabra Datos), variable(s), especie (o grupo) e isla (o región geográfica). E.g. `Censo_Nidos_Albatros_Guadalupe`, `Busqueda_Madrigueras_AvesMarinas_PacificoNorte`, etc. Además, no uses espacios, usa guion bajo '_'.

- **Usa el formato `DD/MMM/AAAA` para todas las fechas** Por ejemplo, `07/Oct/1998`, `01/Ene/2000`, etc.

- **Ten cuidado con los espacios dentro de las celdas.** Una celda en blanco es diferente de una celda que contiene un solo espacio. Y "` macho`" es diferente de "` macho `" (es decir, con espacios en el principio y fin). Estos pueden ser un dolor de cabeza más adelante.

---

Siguiente: [Metadatos](pages/metadatos.html).

(Anterior: [Datos](pages/datos.html).)
