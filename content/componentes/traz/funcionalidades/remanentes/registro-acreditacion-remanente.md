---
title: "Registro de acreditación de remanentes"
date: 2023-10-01T18:30:00-03:00
draft: false
weight: 1
---

El registro podrá realizarse de forma **manual** o **automática**.

## Registro manual

Si no hay una acreditación de remanentes para el origen que corresponda (guías o acreditaciones), se podrá registrar una desde la interfaz. Quedará deshabilitada cuando contenga al menos un producto.

| Pasos                                                                                                                                                                                                                                                                                                                                                                   | Imagen                                                                                                   |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Desde el rol **TRAZ_PUB_ALA** se accederá al menú de remanentes de acreditaciones.                                                                                                                                                                                                                                                                                      | ![registrar acreditación de remanentes manual 1](../images/registro-acreditacion-remanentes-manual1.png) |
| Se debe seleccionar el establecimiento que corresponda.                                                                                                                                                                                                                                                                                                                 | ![registrar acreditación de remanentes manual 2](../images/registro-acreditacion-remanentes-manual2.png) |
| Registrar la nueva acreditación de remanentes desde el botón “Nueva acreditación”. Se pedirá una confirmación y mostrará los datos de la acreditación creada.<br/><br/>{{% notice style="tip" title="Tener en cuenta" %}}Si la acreditación le corresponde a una guía, el código será ACREM-G. Si es de acreditaciones externas, el código será ACREM-A.{{% /notice %}} | ![registrar acreditación de remanentes manual 3](../images/registro-acreditacion-remanentes-manual3.png) |

## Registro automático

La condición para que esto ocurra es que el establecimiento titular de la guía base no tenga previamente una acreditación de remanentes.

| Pasos                                                                                                                                                                                                                                              | Imagen                                                                                                           |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Si se ejecuta la transformación de productos en una guía base de removido y ésta genera subproductos, la acreditación se creará automáticamente con los subproductos asignados y quedará disponible y habilitada para la asignación de remanentes. | ![registrar acreditación de remanentes automático 1](../images/registro-acreditacion-remanentes-automatico1.png) |
