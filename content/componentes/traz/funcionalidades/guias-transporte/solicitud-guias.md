---
title: "Solicitud de guías"
date: 2023-10-01T17:32:00-03:00
draft: false
weight: 1
---

Desde un usuario **TRAZ_PRIV** podremos solicitar al **TRAZ_PUB_ALA** el registro de una guía de transporte.

## Menú de solicitud de guías

| Pasos                                                                                                                                                                                                                          | Imagen                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------- |
| Desde el usuario **TRAZ_PRIV** acceder a _Guías/Solicitar_.                                                                                                                                                                    | ![solicitar guía 1](../images/solicitar-guia1.png) |
| Se establecen los parámetros:<br/><br/><ul><li>Componente local</li><li>Tipo de movimiento</li><li>Establecimiento</li></ul><br/><br/>y finalmente se hace click en el botón “Solicitar nueva guía“.                           | ![solicitar guía 2](../images/solicitar-guia2.png) |
| Una vez abierto el wizard de solicitud, los pasos a completar dentro de él son similares a los del **registro de guía**.                                                                                                       |                                                    |
| Para que la guía pueda ser validada, debemos agregarle **ítems productivos**.<br/><br/>Lo podemos hacer al ingresar al menú de ítems productivos, mediante el botón con ícono de lápiz, en la fila de la guía que corresponda. | ![solicitar guía 3](../images/solicitar-guia3.png) |
| Una vez dentro del menú de ítems productivos, creamos un nuevo ítem y seguimos los pasos del wizard. El proceso es similar al de agregado de productos del registro de guía.                                                   | ![solicitar guía 4](../images/solicitar-guia4.png) |
| Al finalizar los pasos, la guía solicitada deberá ser validada desde el usuario **TRAZ_PUB_ALA**.                                                                                                                              |                                                    |

## Validación de guías solicitadas

Desde el usuario **TRAZ_PUB_ALA** podremos validar o rechazar las solicitudes de guías recibidas de los usuarios **TRAZ_PRIV**.

| Pasos                                                                                                                                                                                                                                      | Imagen                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------- |
| Desde el usuario **TRAZ_PUB_ALA** acceder a Guías/Validar.                                                                                                                                                                                 | ![validar guía solicitada 1](../images/solicitud-guia1.png) |
| Ingresar el CUIT del titular de la guía solicitada y luego completar los campos de “Tipo de movimiento” y “Establecimiento”.<br/><br/>Se listarán las solicitudes de guía recibidas en la parte inferior del menú.                         | ![validar guía solicitada 2](../images/solicitud-guia2.png) |
| Al clickear en el botón de “acciones” de una guía entraremos a su wizard de validación.                                                                                                                                                    | ![validar guía solicitada 3](../images/solicitud-guia3.png) |
| En este wizard podremos ver los ítems asignados a la guía, junto a sus propiedades, detalles de piezas y descuentos.<br/><br/>Mediante los botones verdes podremos _rechazarla_ o _verificarla_.                                           | ![validar guía solicitada 4](../images/solicitud-guia4.png) |
| En caso de **rechazarla**, se pedirá una confirmación. Una vez confirmado el rechazo, se cerrará el wizard, retornando al menú previo y su nuevo estado de “Rechazada” se listará en el menú de guías solicitadas del usuario _TRAZ_PRIV_. | ![validar guía solicitada 5](../images/solicitud-guia5.png) |
| En caso de **verificarla**, se procede a los siguientes pasos del wizard, donde acreditaremos subproductos, si los tuviese.                                                                                                                | ![validar guía solicitada 6](../images/solicitud-guia6.png) |
| Finalmente la guía pasará a tener estado de “Registrada” tanto en el listado de **TRAZ_PRIV**, dentro de su menú de solicitud de guías, como en **TRAZ_PUB_ALA**, dentro de su menú de registro de guías.                                  | ![validar guía solicitada 7](../images/solicitud-guia7.png) |
