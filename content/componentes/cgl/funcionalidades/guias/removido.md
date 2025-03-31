---
title: "Gestión de Guías de Removido"
date: 2023-10-12T18:31:49-03:00
draft: false
weight: 3
---

Como se indicó en la Sección de Guías base de EXTRACCION, el acceso a para la gestión de guías es el mismo para todos los tipos de guías 

![botón cámara](../images/menu_gestionar.png)

Desde el cual se puede editar una guía base existente o crear una nueva

![botón cámara](../images/form_gestion.png)

Se debe tener en cuenta que las fuentes de productos para las guías base de REMOVIDO se obtienen de los que hayan sido acreditados mediante remitos recibidos. De modo que esta información, como la correspondiente al titular y establecimiento origen, surge del componente TRAZ, mediante los servicios correspondientes.  

###### Crear nueva
Desde el botón *Crear nueva* se abre el formulario de creación

| Pasos                         | Imágenes                                |
| ----------------------------- | --------------------------------------- |
| DSe debe seleccionar el tipo de guía base correspondiente, que ya debe estar configurada, y luego definir si el destino de los productos que se reservarán serán transportados fuera o dentro de la provincia | ![botón cámara](../images/form_nueva_2.png) |
| Esto habilitará el campo para ingresar el CUIT del Actuante | ![botón cámara](../images/form_cuit_act.png)|
| Si el CUIT pertenece a un Actuante validado en TRAZ se mostrarán sus datos y si tiene productos acreditados, se listarán los Establecimientos origenes | ![botón cámara](../images/list_est_disp.png)|
| Desde el botón de la derecha se podrá ver el detalle del Etablecimiento seleccionado y el listado de productos disponibles, de Acreditaciones y de remitos recibidos | ![botón cámara](../images/est_selec_gral.png)|
| Si el Establecimiento seleccionado como fuente es adecuado se podrá guardar la guía, en caso contrario se podrá limpiar la selección y revisar otras posibles fuentes | ![botón cámara](../images/guardado_guia_rem.png)|
| Una vez guardada la guía base, se muestra el mensaje y, a la izquierda, el número de la guía nueva y el menú para continuar su registro, que se mostrará en la edición | ![botón cámara](../images/guia_rem_registrada.png)|

###### Editar existente
Los pasos de edición son los mismos que para la continuación del registro de una guía iniciada. Se debe ingresar el código de la guía en el formulario mostrado arriba.

![botón cámara](../images/buscar_guia_rem.png)

Desde el botón buscar, se mostrarán los datos generales de la guía (*como al final de su registro*), editables aún porque no tiene productos asignados

![botón cámara](../images/edit_guia_rem_1.png)

Si se editan los datos generales se volverá al mismo formulario de registro. No se podrá modificar el tipo de guía.

A continuación se muestran los pasos para la gestión del resto de los atributos de la guía base de REMOVIDO que se harán desde el menú lateral a la izquierda.

| Pasos                         | Imágenes                                |
| ----------------------------- | --------------------------------------- |
| **Productos** se accede desde el menú lateral, muestra el listado de productos disponibles y los asignados. Los disponibles, agrupados según su fuente: Acreditaciones, guías o remitos recibidos | ![botón cámara](../images/list_prod_rem_disp.png) |
| **Descontar productos** Desde el botón correspondientes, se accede al formulario | ![botón cámara](../images/btn_descontar_prod.png) 
| Se ingresa la cantidad a descontar teniendo en cuenta que no supere el saldo disponible | ![botón cámara](../images/form_asign_prod_rem.png) |
| Una vez asignado el producto, se mostrará en el listado de asignados y el fuente no podrá tener más descuentos, tampoco se podrá editar los datos generales de la guía. | ![botón cámara](../images/list_prod_asign_rem.png) |
| Como en el caso de las guías de REMOVIDO, se pueden agregar varios descuentos a un mismo item, para hacer una edición hay que seleccionar el descuento del listado de los existentes | ![botón cámara](../images/list_desc.png) |
| Ahí sí, desde el botón de edición del producto asignado, se podrá editar o eliminar el descuento | ![botón cámara](../images/edit_desc_rem.png) |
| **Transformar productos** se procede desde el botón correspondiente, se validará que el producto tenga saldo, mas allá de que haya tenido descuentos | ![botón cámara](../images/btn_transf_prod.png) |
| Se muestra el formulario con el detalle del producto original y el proceso de transformación | ![botón cámara](../images/form_tranf_1.png) |
| A medida que se avance en los grados de transformación se irá actualizando el máximo a obtener | ![botón cámara](../images/form_tranf_2.png) |
| Cuando se llegó a la clase a llegar, que debe estar configurada previamente, se podrá aplicar la transformación con la opción de modificar la cantidad a obtener | ![botón cámara](../images/form_tranf_valid.png) |
| Se mostrará el resumen de los cambios a ejecutar y la posibilidad de ver los subproductos obtenidos, que se acreditarán cuando se ejecute la transformación | ![botón cámara](../images/form_tranf_confirm.png) |
| Se muestra el mensaje con el resumen de la transformación realizada | ![botón cámara](../images/mensaje_transf.png) |
| Se actualiza el listado de las fuentes de productos, permitiendo descontar directamente el saldo restante del transformado | ![botón cámara](../images/list_fuente_act.png) |
| Se muetra la Acreditación de remanentes generada automaticamente para los subproductos generados durante la transformación, que estarán disponibles para su asignación a la guía también | ![botón cámara](../images/list_acred.png) |
| Finalmente, se muestra el listado actualizado de los productos asignados, en el caso del transformado, desde el botón correspondiente, se podrá ver el listado de subrpoductos generados | ![botón cámara](../images/list_prod_asign_tranf.png) |
| En el caso de las asignaciones de productos transformados, solo se podrán eliminar, y eventualmente, hacer la transformación que corresponda | ![botón cámara](../images/detalle_tranf.png) |


Si hay **Tasas** configuradas, se liquidarán de la misma manera que en EXTRACCION

Finalmente, la **Emisión** y la **Extensión de vigencia** serán iguales que en el caso de EXTRACCION