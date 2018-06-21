---
layout: page
title: Resumen
description: datos en excel
---

- Los datos de una actividad de monitoreo se guardan en una o varias tablas de datos.
- Cada tabla de datos se guarda en un archivo de Excel distinto, es decir, cada archivo de Excel contiene una única tabla de datos.
- Cada archivo de Excel debe tener dos hojas: la primera para los datos y la segunda para los metadatos.
- En la hoja de datos, cada columna representa una variable y cada renglón representa una observación.
- En la hoja de los metadatos, cada renglón representa una variable y cada columna representa un conjunto de metadatos.

Ejemplo:

_Tabla: Hoja de datos_

**lat**   | **lon**     | **conteo**
----------|-------------|-----------
31.857778 | -116.605833 | 63
31.858147 | -116.601270 | 27
31.859058 | -116.609134 | 54


_Tabla: Hoja de metadatos_

**name**   | **nombre_largo** | **long_name** | **standard_name** | **axis** | **titulo**                                             | **title**
-----------|------------------|---------------|-------------------|----------|--------------------------------------------------------|------------------------------------
**TABLA**  | NA               | NA            | NA                | NA       | Muestreo por cuadrantes de madrigueras de aves marinas | Quadrat sampling of seabird burrows
**lat**    | Latitud          | Latitude      | latitude          | Y        | NA                                                     | NA
**lon**    | Longitud         | Longitude     | longitude         | X        | NA                                                     | NA
**conteo** | Madrigueras      | Burrows       | NA                | NA       | NA                                                     | NA

---

&rarr; Siguiente: [Datos](datos.html).

&uarr; Inicio: [Contenido](../index.html).
