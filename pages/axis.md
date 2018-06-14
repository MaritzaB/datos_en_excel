---
layout: page
title: Variables independientes
description: Metadato `axis`
---

Para indicar que una columna representa una variable independiente se usa el metadato `axis`.

_Tabla: Posibles valores para `axis`, descripción de variables y posibles valores para `standard_name`._

`axis` | Variable                              | `standard_name` válidos
:-----:|:--------------------------------------|:---------------------------------------
C      | ID de la colonia o islote             |
I      | Isla o islote                         |
N      | ID del nido o madriguera              | `nest_id`
P      | ID del punto o sitio de avistamiento  | `point_id`
R      | Anillo del individuo                  |
S      | Especie                               | `common_name`, `scientific_name`
T      | Tiempo (fecha y hora)                 | `time`, `date`, `datetime`
X      | Cooredenada zonal                     | `longitude`, `projection_x_coordinate`
Y      | Coordenada meridional                 | `latitude`, `projection_y_coordinate`
Z      | Altitud                               | `altitude`

---

Siguiente: [Sistema de Coordenadas](coordenadas.html).

(Anterior: [Nombre estándar](standard_name.html).)