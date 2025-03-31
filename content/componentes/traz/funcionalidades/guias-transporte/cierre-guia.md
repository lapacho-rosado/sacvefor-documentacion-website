---
title: "Cierre de guía emitida"
date: 2023-09-27T10:42:00-03:00
draft: false
weight: 4
---

{{% notice style="note" title="Tener en cuenta" %}}

- La guía debe ser cerrada por el destinatario y sólo podrá hacerlo mientras no se haya vencido su vigencia.
- Debe estar creado el usuario para el destinatario de la guía y tener accesibles sus credenciales de acceso.
  {{% /notice %}}

## Menú de cierre de guías

| Pasos                                                                                                                                                                                                                       | Imagen                                          |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| Desde el rol TRAZ_PRIV, el destinatario de la guía debe acceder a Guia/Cerrar                                                                                                                                               |                                                 |
| Se listarán las guías pendientes de cierre, entre las que deberá estar la guía emitida. De cada una se podrá acceder al detalle de la guía mediante el botón del ojo o directamente al cierre mediante el botón de candado. | ![cierre de guía 1](../images/cierre-guia1.png) |
| Si se accede al detalle se muestra un modal con los detalles de la guía y tres botones:                                                                                                                                     | ![cierre de guía 2](../images/cierre-guia2.png) |
| Muestra el detalle de los productos que contiene la guía.                                                                                                                                                                   | ![cierre de guía 3](../images/cierre-guia3.png) |
| Muestra las fuentes de los productos, en este caso, la guía base del CGL.                                                                                                                                                   | ![cierre de guía 4](../images/cierre-guia4.png) |
| Muestra el mensaje de confirmación de cierre.                                                                                                                                                                               | ![cierre de guía 5](../images/cierre-guia5.png) |
| Si se accede al cierre directamente desde la guía listada, se muestra el mismo mensaje de confirmación.                                                                                                                     | ![cierre de guía 6](../images/cierre-guia6.png) |
| Al confirmar el cierre, se retorna al listado de guías a cerrar, que ya no mostrará la guía cerrada.                                                                                                                        |                                                 |

---

## Verificación en TRAZ

| Pasos                                                                      | Imagen                                                              |
| -------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| Desde el rol \_TRAZ*PUB_ALA, acceder al menú \_Consulta/Guías acreditadas* |                                                                     |
| Seleccionar el período que incluya la fecha de cierre y buscar             | ![verificar cierre de guía 1](../images/verificar-cierre-guia1.png) |
| Se listarán las guías acreditadas, entre las que deberá estar la cerrada.  | ![verificar cierre de guía 2](../images/verificar-cierre-guia2.png) |

## Verificación en CGL

Si la guía de transporte cerrada era de _removido_ se puede verificar que esté disponible como fuente de productos. Para eso se puede ver el inicio de una guía base de removido para el establecimiento destino desde el CGL.

| Pasos                                                                                                                                                                    | Imagen                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------- |
| Setear los parámetros para la creación de la guía.<br/><br/><ul><li>Tipo de guía: REMOVIDO</li><li>CUIT del Actuante: [el del destinatario de la guía cerrada]</li></ul> |                                                                                          |
| Al buscar se mostrará el Establecimiento destino.                                                                                                                        |                                                                                          |
| Al buscar los productos disponibles se listarán los acreditados desde la guía de transporte cerrada. (no es necesaria la creación de una nueva guía base)                | ![verificar cierre de guía de removido 1](../images/verificar-cierre-guia-removido1.png) |
