---
title: "Gestión de Guías de Extracción"
date: 2023-10-12T18:31:36-03:00
draft: false
weight: 2
---

Tanto para gestionar guías base de *EXTRACCION* como de *REMOIVIDO* se accede desde el menú *Guías/Gestionar*

![botón cámara](../images/menu_gestionar.png)

Desde aquí se puede editar una guía base existente o crear una nueva

![botón cámara](../images/form_gestion.png)

###### Crear nueva
Desde el botón *Crear nueva* se abre el formulario de creación

| Pasos                         | Imágenes                                |
| ----------------------------- | --------------------------------------- |
| Se debe seleccionar el tipo de guía base correspondiente, que ya debe estar configurada, y luego definir si el destino de los productos que se reservarán serán transportados fuera o dentro de la provincia | ![botón cámara](../images/form_nueva_1.png) |
| Esto habilitará el campo para ingresar el CUIT del Productor | ![botón cámara](../images/form_cuit.png)|
| Si el CUIT pertenece a un productor registrado se mostrarán sus datos y si tiene Autorizaciones vigentes con productos, se liestarán | ![botón cámara](../images/list_aut_disp.png)|
| Desde el botón de la derecha se podrá ver el detalle de la Autorización seleccionada | ![botón cámara](../images/aut_selec_gral.png)|
| Si tiene rodales disponibles se deberá asignar alguno | ![botón cámara](../images/aut_rodales_disp.png)|
| Y se mostrará el listado con los productos disponibes, mostrando su saldo | ![botón cámara](../images/aut_select_prod.png)|
| Al guardar la fuente seleccionada, se muestra el mensaje y permitirá guardar la guía o limpiar todo | ![botón cámara](../images/guardado_guia_ext.png)|
| Una vez guardada la guía base, se muestra el mensaje y, a la izquierda, el número de la guía nueva y el menú para continuar su registro, que se mostrará en la edición | ![botón cámara](../images/guia_registrada.png)|
 
###### Editar existente
Los pasos de edición son los mismos que para la continuación del registro de una guía iniciada. Se debe ingresar el código de la guía en el formulario mostrado arriba.

![botón cámara](../images/buscar_guia.png)

Desde el botón buscar, se mostrarán los datos generales de la guía (*como al final de su registro*), editables aún porque no tiene productos asignados

![botón cámara](../images/edit_guia_1.png)

Si se editan los datos generales se volverá al mismo formulario de registro. No se podrá modificar el tipo de guía.

A continuación se muestran los pasos para la gestión del resto de los atributos de la guía base que se harán desde el menú lateral a la izquierda.


| Pasos                         | Imágenes                                |
| ----------------------------- | --------------------------------------- |
| **Obrajeros** (*si están configurados*) Se muestra el formulario para ingresar el CUIT | ![botón cámara](../images/form_obrajeros.png) |
| Si el CUIT ingresado pertenece a un Obreajero vigente, se lo mostrará y se podrá agregar | ![botón cámara](../images/obraj_encontrado.png) |
| Una vez agregado o al editar con un obrajero existente, se lo podrá modificar desde el listado | ![botón cámara](../images/list_obrajeros.png) |
| **Asignar Productos** se accede desde el menú lateral. Si aún no se asignaron productos, mostrará un SELECT con los productos con saldo disponible provenientes de la Autorización. Si ya se asignaron productos, mostrará debajo el listado correspondiente  | ![botón cámara](../images/select_prod_disp.png) |
| El listado muestra un resumen de los productos disponibles conteniendo *Especie - Clase - Unidad de medida*. Se podrá seleccionar el producto que corresponda y continuar | ![botón cámara](../images/select_prod_disp_desplegado.png) |
| Una vez seleccionado el producto se mostrarán los detalles del producto seleccionado y los pasos a seguír según la configuración del mismo. Si solo permite descuento de saldo, mostrará el botón *Descontar*. | ![botón cámara](../images/btn_descontar_prod_ext.png) |
| Si el producto seleccionado permite descuento y transformación directa, además se mostrará el botón *Transformar*. | ![botón cámara](../images/btn_transformar_prod_ext.png) |
| Desde el botón *Descontar* se accede al formulario en el cual habrá que especificar la cantidad a descontar y guardar. Validará que no supere al saldo disponible | ![botón cámara](../images/form_asign_prod_ext.png) |
| Desde el botón *Transformar* se accede al formulario de transformación que lista las clases configuradas disponibles a obtener, para seleccionar la que corresponda | ![botón cámara](../images/form_tranf_ext_select_clase.png) |
| Una vez seleccionada la clase a obtener se mostrará el máximo disponible para asignar cantidad | ![botón cámara](../images/form_tranf_ext_asign_cant.png) |
| Una vez asignada cantidad se mostrará el resumen de lo obtenido mediante la transformación, el descuento a realizar y el saldo a actualizar. Se podrá retroceder para modificar o ejecutar la transformación | ![botón cámara](../images/form_tranf_ext_cant_confirm.png) |
| Una vez ejecutada la transformación o el descuento directo, desde el listado de productos asignados se podrá *Editar* el descuento o *Eliminar* la transformación, según corresponda | ![botón cámara](../images/list_prod_asign_extrac.png) |
| Una vez asignado una cantidad de producto no permitirá una nueva asignación, solo permitirá la selección para hacer transformación directa, si está disponible para el producto | En caso de permitir transformación se validará la no selección de una clase ya obtenida mediante transformación |
| Si se seleccionó un producto ya asignado para su modificación, se podrá editar o eliminar el descuento desde un formulario similar al de asignación | ![botón cámara](../images/edit_desc_extrac.png) |
| **Tasas** se accede desde el menú lateral, muestra el detalle por productos, por unidad y por cantidad. Los productos deben tener tasas configuradas. Desde el botón *Generar Resumen* se generará el reporte en .PDF con las tasas liquidadas quedando en situación de emisión | ![botón cámara](../images/detalle_tasas.png) |

###### Emitir
Una vez que la guía haya liquidado las tasas quedará en condiciones de ser emitida, para lo cual, en el menú lateral izquierdo se mostrará el correspondiente a la emisión

![botón cámara](../images/menu_emitir.png)

| Pasos                         | Imágenes                                |
| ----------------------------- | --------------------------------------- |
| Se deberá ingresar el código compprobante del recibo de pago de las tasas | ![botón cámara](../images/cod_recibo.png) |
| Al registrar el código, se mostrarán los datos generales de la guía base a emitir junto con el listado de productos | ![botón cámara](../images/emitir_ext.png) |
| Una vez que la guía haya sido emitida, quedará en condiciones de ser usada como fuente de productos para remnitos de transporte y, mientras esté vigente se podrá extender la vigencia | ![botón cámara](../images/guia_emitida.png) |

###### Extender vigencia
Una vez que la guía base sea emitida puede ocurrir que se venza su vigencia pero aún quede con saldo de productos asignados, esto se resolverá con la extensión de la vigencia.

Desde el menú lateral se muestra el formulario que requerirá una razón y que la fecha actualizada sea posterior a la de vencimiento original.

![botón cámara](../images/extender_vig.png)

Al aceptar, se imprime un nuevo reporte de guía con la fecha de vencimiento y los saldos de productos actualizados. Además se notifica por correo electrónico la novedad al tiitular.
