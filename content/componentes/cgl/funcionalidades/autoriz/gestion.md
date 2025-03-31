---
title: "Gestión y vista"
date: 2023-10-12T18:10:46-03:00
draft: false
weight: 3
---

Aquí se describen las funcionalidades de Gestión de las Autorizaciones y el acceso al listado de las existentes

![botón cámara](../images/gestion_aut.png)

Desde la *Gestión* se puede acceder a la creación de una nueva Autorización y la edición de una existente:

![botón cámara](../images/gestion_aut_2.png)

En el caso de crear una nueva aparecerá el formulario inicial en el que se deberá registrar:

| Elementos                     | Descripción                                |
| ----------------------------- | ------------------------------------------ |
| Instrumento Legal Aprobatorio | Número del instrumento legal y la fecha de aprobación (*el formato del número y el tipo de Instrumento son configurables*) |
| Expediente | Número del expediente que solicitó la Autorización y la fecha de ingreso (*el formato del número del expediente es configurable*) |
| Autorización | Se selecciona el tipo de intervención, el uso del suelo, si pertenece a una Cuenca forestal y se registra la fecha de vencimiento |
| Predio | Se ingresan la superficie total, la solicitada y la autorizada, que es la fundamental. Además se selecciona la Zona y si corresponde, la sub zona |
| Observaciones | Se suele usar más para objetos editados o con vigencia extendida |

Una vez que se guarde la Autorización se mostrará el menú de la izquerda con el número y los elementos a gestionar:

![botón cámara](../images/aut_menu_lat.png)

Cada objeto del menú lateral muestra el listado y formulario de los objetos citados, salvo el primero, que muestra un formulario similar al del registro de la Autorización y pemite su edición, mientras el estado lo permita.

| Elementos                     | Descripción                                |
| ----------------------------- | ------------------------------------------ |
| Proponentes | Muestra el listado y formularios para la gestión de proponentes. Se selecciona por el cuit |
| Apoderados | Muestra el listado y formularios para la gestión de Apoderados (*Opcional*). Se selecciona por el cuit |
| Técnicos | Muestra el listado y formularios para la gestión de técnicos. Se selecciona por el cuit |
| Inmuebles | Muestra el listado y formularios para la gestión de inmuebles. Se selecciona por el id catastral |
| Productos forestales | Se selecciona la especie y luego la clase ![botón cámara](../images/aut_productos.png) finalmente se asigna cantidad y se guarda ![botón cámara](../images/aut_productos_2.png) |
| Estado | En principio será de *Carga inicial* y cuando esté completa se la pasará a *Habilitada*. ![botón cámara](../images/carga_inical.png) Una vez habilitada, no se podrá editar, solo se podrá volver a Carga inicial mientras no se le descuenten productos|


Las Autorizaciones registradas estarán disponibles desde el menú ver:

![botón cámara](../images/vista_aut.png)

Muestra el listado y un formulario de búsqueda por CUIT y nombre de Proponente:

![botón cámara](../images/vista_buscar.png)

Desde cada Autorización listada se podrá acceder a su detalle:

| Elementos                     | Descripción                                |
| ----------------------------- | ------------------------------------------ |
| Detalle | Muestra el detalle de los datos generales de la Autorización ![botón cámara](../images/aut_vista_detalle.png) |
| Personas vinculadas | Muestra el listado con las personas vinculadas según sus roles ![botón cámara](../images/aut_vista_personas.png) |
| Inmuebles vinculados | Muestra el listado con los inmuebles, se puede acceder a Rodales o Cuarteles ![botón cámara](../images/aut_vista_inmuebles.png) |
| Productos autorizados | Muestra el listado de los productos autorizados con los saldos que se vayan actualizando ![botón cámara](../images/aut_vista_productos.png) Desde cada productos se podrán ver los descuentos otorgados |
| Ver Guías | Finalmente, desde el botón correspondiente se podrán ver las guías base generadas que descontaron productos desde la Autorización ![botón cámara](../images/aut_guias.png) |