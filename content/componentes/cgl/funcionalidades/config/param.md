---
title: "Parámetros"
date: 2023-10-12T11:46:27-03:00
draft: false
weight: 1
---

En el caso de tener el rol de **Administrador** en el CGL se pueden realizar las siguientes configuraciones de parámetros:

##### Autoridad local
Se agregó esta configuración para vincularse con la nueva versión del Componente de Trazabilidad (TRAZ). Incluye la información que se muestra en los correos, en los reportes y en el pie de página de la aplicación. Se accede desde el menú Administración/Autoridad local.

![botón cámara](../images/menu_admin.png)

Se configura una sola vez y requiere información solicitada por la Administración central del SACVeFor para los tres primeros atributos, los restantes son los definidos por la Autoridad local.

![botón cámara](../images/aut_local.png)

Debe tenerse en cuenta que la clave de acceso al servicio (clave TRAZ) no se muestra en el formulario, pero si se hace alguna actualización deberá ser ingresada para que se guarden los cambios.

##### Información general
Al iniciar sesión se accederá a la vista inicial de la aplicación desde la cual se podrá acceder a mensajes de información general destinada a los usuarios. La actualización de esta información se podrá realizar desde el menú **Administración/Información general**. Desde donde se mostrará el formulario correspondiente:

![botón cámara](../images/info_gral.png)

##### Tipos de parámetros
Se trata del tipo de Parámetros generales de administración (consistentes en un id y un nombre).  Los básicos en la vesrión 2 serán los siguientes:

- CUENCA_FORESTAL: Nombres de las Cuencas que pudiera haber en la provincia
- DEST_GUIAS: Destinos de los productos transportados, dentro o fuera de la provincia
- DISC_TASA: Para los casos en que haya tasas que se liquiden de forma discriminada, agrupa esos casos
- PLAN_INTEGRAL: Tipos de planes integrales de intervención forestal
- ROL_PERSONAS: Diferentes roles que las personas privadas pueden tener en la aplicación
- ROL_USUARIOS: Diferentes roles que los usuarios pueden tener en la aplicación
- TIPO_AUTORIZACION: instrumento legal que utilice la provincia  
- TIPO_FUENTE: Diferentes fuentes de productos para una Guía BASE
- TIPO_INTERVENCION: Diferentes intervenciones forestales que la ALA pueda autorizar
- TIPO_ITEM: Diferentes tipos de items productivos, de autorizaciones y de distintos tipos de guías base
- TIPO_MOV: Posibles movimientos de productos: PRIMERO, REMOVIDO
- TIPO_NUMERICO: Tipos de número a configurar: enteros, decimales
- TIPO_TASA: Diferentes tipos de tasa que se pueden asignar a prodictos y liquidar con las guías base.
- TIPO_TRANSF: Diferentes transformaciones de productos que se pueden ejecutar en las guías base de removido
- USO_SUELO: Diferentes usos del suelo que se pueden asignar a tipos de intervención

El uso de algunos como CUENCA_FORESTAL o DISC_TASA pueden ser opcionales, pero se recomienda su configuración.</br> 
La actualización de esta información se podrá realizar desde el menú **Administración/Tipos de Parámetros** que muestra el formulario en el cual solo se ingresará el nombre. 

![botón cámara](../images/form_tipo_param.png)

Tal nombre está configurado también en archivos de la aplicación, de modo que deben tener el formato mostrado arriba. De ser necesario un cambio o un agregado, deberá ser coordinado con la Administración general del Sistema.

Dede el listado de los objetos registrados, como en la mayoría de los casos de los listados, se podrá ver el detalle, editar y habilitar o deshabilitar, según el caso.

| Acciones                                  | Imagen                                 |
| ----------------------------------------- | -------------------------------------- |
| Ver detalle                               | ![botón cámara](../images/btn_ver.png) |
| Editar                                    | ![botón cámara](../images/btn_edit.png) |
| Deshabilitar (si está habilitado)         | ![botón cámara](../images/btn_hab.png) |
| Habilitar (si está deshabilitado)         | ![botón cámara](../images/btn_deshab.png) |

##### Entidades paramétricas
Se trata de parámetros genéricos de la aplicación del tipo id, nombre y tipo, siendo el tipo, el detallado en el punto anterior. A modo de ejemplo se muestran los básicos:

| Tipo de parametro                         | Parametros                                 |
| ----------------------------------------- | ------------------------------------------ |
| CUENCA_FORESTAL | Si corresponde, lo define la Autoridad local |                          
| DEST_GUIAS                                | EXTERNO, INTERNO |
| DISC_TASAS | DEST_GUIAS, ORIGEN_PREDIO, TIPO_INTERVENCION (deben estar configuradas como tipo de parámetro previamente)| 
| ORIGEN_PREDIO | Si corresponde, los define la Autoridad local |
| ROL_PERSONAS | APODERADO, PROPONENTE, TECNICO, OBRAJERO |
| ROL_USUARIOS | ADMINISTRADOR, COORDINADOR, REGISTRADOR DE AUTORIZACIONES, REGISTRADOR DE GUIAS |
| TIPO_AUTORIZACION | RESOLUCION o DISPOSICION |
| TIPO_FUENTE | ACREDITACION, AUTORIZACION, REMITO DE TRANSPORTE |
| TIPO_INTERVENCION | PLAN MANEJO SOSTENIBLE, CAMBIO USO DEL SUELO, MANEJO FORESTAL/APROVECHAMIENTO FORESTAL |
| TIPO_ITEM | AUTORIZADOS, EXTRAIDOS, REMOVIDOS |
| TIPO_MOV | PRIMER MOVIMIENTO, REMOVIDO |
| TIPO_TASA | RENTAS REMOVIDO, EXTENSION VIGENCIA, AFORO FISCAL |
| USO_SUELO | APROVECHAMIENTO FORESTAL, CAMBIO DE USO, DESMONTE |

Como en el caso de los tipos de parámetros, los nombres está configurados también en archivos de la aplicación, de modo que deben tener el formato mostrado arriba. De ser necesario un cambio o un agregado, deberá ser coordinado con la Administración general del Sistema.

La actualización de esta información se podrá realizar desde el menú **Administración/Entidades Parámétricas** que muestra el formulario en el cual se selecciona el tipo de parametro y se asigna el nombre.

![botón cámara](../images/form_param.png)

Dede el listado de los objetos registrados, como en la mayoría de los casos de los listados, se podrá ver el detalle, editar y habilitar o deshabilitar, según el caso.

##### Estados de Guía
Los estados de guía estarán listos desde la primera configuración del CGL para la provincia, en caso de ser necesario algún cambio, será coordinado desde la Administración general del Sistema.

##### Tipo de Guía
Se trata de los tipos de guías que se tramitan en una Provincia determinada gestionadas mediante el componente local del SACVeFor. Serán solo guías de fiscalización previa, no ampararán transporte de forma directa. Basicamente serán diferenciadas por el tipo de movimiento que ampararán. La actualización de esta información se podrá realizar desde el menú **Administración/Tipos de Guía** que muestra el formulario en el cual se hace el registro según lo que se describirá a continuación.

![botón cámara](../images/form_tipo_guia.png)

El nombre será definido por la ALA, ya deben estar configurados los parámetros TIPO_MOV, que se listarán en tipo de movimiento, según el cual se procederá:

| Pasos                                                 | Imagenes                                   |
| ----------------------------------------------------- | ------------------------------------------ |
| PRIMER MOVIMIENTO: Descuenta de Autorización          | ![botón cámara](../images/form_tipo_guia_prim.png) |
| REMOVIDO: No descuenta de Autorización, podrá ser pública, pero aún no están habilitadas en TRAZ | ![botón cámara](../images/form_tipo_guia_rem.png) |
| Configuración de tasas: Si el tipo de guía requiere tener tasa asociadas se mostrará el botón que abre el formulario de configuración | ![botón cámara](../images/form_tipo_guia_tasas.png) |
| Se listarán los parámetros TIPO_TASA que estén configurados | ![botón cámara](../images/form_tipo_guia_form_tasas.png) |
| Una vez seleccionada la Tasa, si discrimina liquidación, según el caso seleccionado, listará los valores posibles | ![botón cámara](../images/form_tipo_guia_tasas_caso_valor.png) |
|Al guardar la tasa configurada, la mostrará en el listado, desde el cual se la podrá eliminar desde el botón ![botón cámara](../images/btn_hab.png) | ![botón cámara](../images/form_tipo_guia_list_tasas.png) |
| Una vez configuradas todas las tasas, se cerrará el formulario y quedará asignar los días de vigencia | ![botón cámara](../images/form_tipo_guia_vigencia.png) |
| Una vez que se configró todo se podrá guardar con el botón correspondiente y aparecerá en el listado | ![botón cámara](../images/form_tipo_guia_list.png) |

Dede el listado de los objetos registrados, como en la mayoría de los casos de los listados, se podrá ver el detalle, editar y habilitar o deshabilitar, según el caso.

##### Copias por Tipo de Guía
Cada tipo de guía deberá tener configuradas las copias que deberán ser emitidas. Según esta configuración, al emitir una guía, el archivo en formato pdf a imprimir contendrá todas las copias configuradas. En la versión de pruebas de la versión 2, para simplificar todo solo se asignó una copía por tipo de guía. La actualización de esta información se podrá realizar desde el menú **Administración/Copias por Tipo de Guía** que muestra el formulario en el cual se hace el registro según lo que se describirá a continuación.

![botón cámara](../images/form_copias_tipo_guia.png)

Deben estar configurados previamente los tipos de guía a los que se les quiere asignar las copias, por cada una se configurará:
- Nombre de la copia (ORIGINAL, DUPLICADO, etc.)
- Destino al cual será dirigida la copia

Al guardar la copia se mostrará en el listado que, como en los casos anteriores, se podrán editar, habilitar o deshabilitar

![botón cámara](../images/list_copias_tipo_guia.png)