---
layout: page
title: Resumen
tagline: para analistas de datos
---

- Recibimos cada tabla de datos en un archivo de Excel que cumple [este protocolo](../index.html)
- Convertimos el archivo de Excel validado a [_Tabular Data Package_ (TDP)](https://frictionlessdata.io/docs/tabular-data-package/)
    - Convertimos la primer hoja de Excel en una tabla de datos CSV
    - Convertimos el segundo renglón de la segunda hoja de Excel en el [descriptor del TDP](https://frictionlessdata.io/specs/tabular-data-package/)
    - Convertimos el resto de la segunda hoja en el [descriptor del recurso de datos tabulados](http://frictionlessdata.io/specs/tabular-data-resource/)
- Importamos el TDP anterior como un objeto `DataTable` (**datatools**)
- Procesamos los datos de forma [reproducible](http://kbroman.org/steps2rr/) siguiendo nuestro [manual de procedimientos](https://bitbucket.org/IslasGECI/analisis/src/default/README.md) y nuestra [guía de estilo](../../ciencia_de_datos/guia_de_estilo.html)
- Entregamos los resultados mediante Trello (evitando enviar archivos adjuntos por correo)

---

&rarr; Siguiente: [Metadatos](metadatos.html)

&uarr; Inicio: [Información adicional para analistas de datos](index.html)
