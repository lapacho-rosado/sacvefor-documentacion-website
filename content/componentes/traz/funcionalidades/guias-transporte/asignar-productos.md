---
title: "Asignar productos a guía"
date: 2023-09-26T20:04:00-03:00
draft: false
weight: 3
---

## Menú de registro de guías

| Pasos                                                                                                                                                                                                                                              | Imagen                                                   |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| Desde el listado de los parámetros de filtro seleccionados se muestra la guía registrada.<br/><br/>Desde el botón “Ver productos” ![botón ver productos](../images/asignar-productos1.png?classes=inline) se accede al listado de ítems asignados. | ![asignar productos 1](../images/asignar-productos2.png) |
| Al clickear en "Nuevo Ítem" se listan los productos fuente disponibles para descontar y agregarlos a la guía.                                                                                                                                      | ![asignar productos 2](../images/asignar-productos3.png) |
| Desde el botón de “Acciones“ seleccionar el item fuente para descontar saldo. Esto abre el wizard con los pasos del registro de ítems productivos.                                                                                                 | ![asignar productos 3](../images/asignar-productos4.png) |

## Wizard de agregado de ítems

| Pasos                                                                                                                                             | Imagen                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| _Seleccionar origen:_ muestra los datos del ítem fuente, especialmente el saldo disponible.                                                       | ![asignar productos 4](../images/asignar-productos5.png) |
| _Asignación de cantidad:_ setear la cantidad a descontar (menor o igual al saldo disponible, entre 1 y 5 está bien).                              | ![asignar productos 5](../images/asignar-productos6.png) |
| _Guardar:_ como estas guías no abonan tasas, se pasa directo al paso 4 que muestra lo que se asignó y el saldo disponible, con sus equivalencias. | ![asignar productos 6](../images/asignar-productos7.png) |
| Se vuelve al listado de ítems asignados a la guía y ya mostrará el ítem agregado.                                                                 | ![asignar productos 7](../images/asignar-productos8.png) |

{{% notice style="tip" %}}
Se recomienda agregar a la guía dos o más ítems al realizar las pruebas.
{{% /notice %}}

---

## Verificar en CGL

Una vez asignados los productos a la guía de transporte, se podrán verificar los descuentos en la guía base origen del CGL de gestión de la guía de transporte.

| Pasos                                                                                                                                                                            | Imagen                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| Acceder al CGL de la ALA de gestión con el usuario de rol COORDINADOR                                                                                                            | ![verificar productos asignados 1](../images/verificar-productos1.png) |
| Desde el menú Guías/Ver se listará la guía base existente.                                                                                                                       | ![verificar productos asignados 2](../images/verificar-productos2.png) |
| Desde el botón de lupa se mostrarán los detalles de la guía seleccionada.                                                                                                        | ![verificar productos asignados 3](../images/verificar-productos3.png) |
| Desde el listado de Detalle de productos, se muestran los productos disponibles con la cantidad asignada y el saldo disponible.                                                  | ![verificar productos asignados 4](../images/verificar-productos4.png) |
| Desde el botón de flecha ascendente de cada ítem productivo descontado se podrá ver el detalle del descuento.                                                                    | ![verificar productos asignados 5](../images/verificar-productos5.png) |
| Se deberá ver el código de la guía de transporte registrada en TRAZ, el id del ítem al que se le asignó el descuento (id ítem destino) y la cantidad asignada (saldo entregado). | ![verificar productos asignados 6](../images/verificar-productos6.png) |
