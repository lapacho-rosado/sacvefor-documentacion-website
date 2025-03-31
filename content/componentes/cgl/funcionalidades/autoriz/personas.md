---
title: "Personas e Inmuebles"
date: 2023-10-12T18:10:30-03:00
draft: false
weight: 2
---

En el caso de tener el rol de **Registrador de Autorizaciones** en el CGL se pueden realizar las siguientes configuraciones de las personas y los inmuebles vinculados a las Autorizaciones.

Con respecto a las personas se debe tener en cuenta que, más allá de ser físicas o jurídicas, y de los roles que puedan tener, son previamente registrados en el servicio *Registro Único de Entidades* (RUE) del Sistema. Y a partir del registro quedan disponibles para cualquier componente.

##### Proponente
El proponente es la persona principal vinculada a una Autorización, puede ser uno o más y se refiere a quien solicita la Autorización para la extracción de productos forestales. Como en el caso de todas las personas, se podrá registrar o seleccionar:

![botón cámara](../images/proponentes_1.png)

- Buscar por CUIT

![botón cámara](../images/buscar_por_cuit.png)

En este caso, se debe ingresar el CUIT y si se encuentra la persona registrada, se mostrarán sus datos y se la podrá seleccionar

![botón cámara](../images/buscar_por_cuit_1.png)

Una vez seleccionado, se muestran sus datos en el formulario de registro del Proponentes y se lo podrá guardar

![botón cámara](../images/buscar_por_cuit_2.png)

- Agregar nuevo

En el caso en que no se haya encontrado a la persona mediante su CUIT en el RUE, se deberá abrir un formulario de registro en el RUE y seleccionar el tipo de persona y registrar los elementos correspondientes. El caso del domicilio, no es obligatorio.

![botón cámara](../images/form_nuevo_RUE_2.png)

Una vez guardada la persona en el RUE, se la podrá seleccionar mediante su CUIT, como ya se describió.

Desde el listado de Proponentes registrados, como en la mayoría de los casos de los listados, se podrá ver el detalle, editar y habilitar o deshabilitar, según el caso.

##### Técnicos
Se trata de Técnicos forestales que representan a los proponentes en la solicitud de Autorizaciones y su gestión. Dado de que se trata de personas, el proceso de registro o selección en RUE es el mismo que el descripto para los Proponentes. Debe tenerse en cuenta que los técnicos, en su formulario, requieren fecha de inicio y fin de vigencia.

![botón cámara](../images/form_tecnico.png)

Desde el listado de Técnicos registrados, como en la mayoría de los casos de los listados, se podrá ver el detalle, editar y habilitar o deshabilitar, según el caso.

##### Apoderados
Se trata de Personas o Entidades que representan a los proponentes en la gestión de los productos provenientes de sus predios. Dado de que se trata de personas, el proceso de registro o selección en RUE es el mismo que el descripto para los Proponentes. Debe tenerse en cuenta que los Apoderados, en su formulario, requieren fecha de inicio y fin de vigencia. Su uso no es obligatorio.

Desde el listado de Apoderados registrados, como en la mayoría de los casos de los listados, se podrá ver el detalle, editar y habilitar o deshabilitar, según el caso.

##### Inmuebles
Con un nombre configurable, en algunos casos *Tramo*, los inmuebles se refieren al lugar en el que se autoriza la extracción de productos. Debe tenerse en cuenta que un mismo inmueble, puede tener más de una Autorización, dadas sus características, sus dimensiones, sus diferencias en zonas. Por tal motivo, se los puede dividir en partes cuyos nombres pueden ser *Cuarteles* o *Rodales*, los cuales se podrán asignar a una Autorización, para especificar más las características del permiso.

Lo primero que se debe definir en un Inmueble es la imagen de *Martillo*, que se muestra en el formulario de registro:

![botón cámara](../images/inmueble_martillo.png)

Una vez que se la seleccione, se la podrá subir y continuar con el formulario de registro:

![botón cámara](../images/form_inmueble.png)

| Parámetros                       | Descripción                                |
| -------------------------------- | ------------------------------------------ |
| Id Catastral | Su formato se configura para cada Provincia |
| Nombre | Nombre de predio |
| Inmueble de origen | Se podrá seleccionar un predio regitrado, del cual se haya obtenido el inmuebe en registro |
| Origen del Inmueble | Parámetro de tipo ORIGEN_PREVIO. Es opcional |
| Cualteles o Rodaes | Son opcionales, si se requiere, se abre un formulario para su registro, solo lleva un número o nombre |
| Domicilio | En el caso que lo tenga, se lo agrega |
| Provincia, Departamenteo, Localidad | Se los selecciona de mayor a menor |
| Superficie | Superficie el predio en *Hectáreas* |
| Latitud y Longitud | Ubicación de un punto que identifique la ubicación de predio |

Luego de guardado, desde el listado de Inmuebles registrados, como en la mayoría de los casos de los listados, se podrá ver el detalle, editar y habilitar o deshabilitar, según el caso.
