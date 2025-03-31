---
title: "Emitir guía registrada"
date: 2023-09-27T10:14:00-03:00
draft: false
weight: 2
---

{{% notice style="note" title="Tener en cuenta" %}}
Para emitir una guía registrada, debe tener al menos un ítem productivo asignado.
{{% /notice %}}

## Menú de emisión de guía

| Pasos                                                                                                                        | Imagen                                                                                       |
| ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Desde el rol TRAZ*PUB_ALA, acceder al menú \_Guia/Registrar*                                                                 |                                                                                              |
| Seleccionar los parámetros de filtro para obtener las guías registradas.                                                     |                                                                                              |
| Desde el listado de guías registradas según los parámetros seleccionados, seleccionar en la guía a emitir el botón “Emitir”. | ![emitir guía 3](/funcionalidades/funcionalidades/primer-movimiento/images/emitir-guia1.png) |

## Wizard de emisión de guía

{{% notice style="info" title="Tener en cuenta" %}}
Como estamos trabajando con ALAs que hacen fiscalización previa (emiten guías base para descontar productos) los pasos 2 y 3 del wizard se ignoran. Esto se debe a que corresponden a la liquidación de tasas.
{{% /notice %}}

| Pasos                                                                                                                                                                                                                                                                                                                                                                                                             | Imagen                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Iniciar: Muestra el listado de ítems productivos asignados, permite ver detalle de piezas (no utilizado en la primera etapa) y los descuentos obtenidos de las fuentes (en este caso, será de la guía base del CGL)                                                                                                                                                                                               | ![emitir guía 2](/funcionalidades/funcionalidades/primer-movimiento/images/emitir-guia2.png) |
| Emitir: Se muestran los datos generales de la guía a emitir y al final, el botón para la generación del PDF.<br/><br/>Al imprimir el PDF, se genera el archivo, se emiten los correos notificando al titular y al destinatario y se actualiza el estado de la guía.<br/><br/>{{% notice style="warning" title="Advertencia" %}}Si no se generó el PDF no se podrá finalizar el proceso de emisión.{{% /notice %}} | ![emitir guía 3](/funcionalidades/funcionalidades/primer-movimiento/images/emitir-guia3.png) |
| Guardar: se retorna al listado de guías registradas según los parámetros de filtro y se muestra un mensaje al usuario indicando que la guía se ha emitido.                                                                                                                                                                                                                                                        | ![emitir guía 4](/funcionalidades/funcionalidades/primer-movimiento/images/emitir-guia4.png) |

---

## Verificación en TRAZ

| Pasos                                                                                 | Imagen                                                                                                             |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Desde el rol TRAZ*PUB_ALA acceder al menú \_Consulta/Guías Remitidas*                 |                                                                                                                    |
| Seleccionar el período que incluya la fecha de emisión y buscar con el botón de lupa. | ![verificar guía emitida 1](/funcionalidades/funcionalidades/primer-movimiento/images/verificar-guia-emitida1.png) |
| Se listarán las guías emitidas, entre las que deberá estar la emitida recién.         | ![verificar guía emitida 2](/funcionalidades/funcionalidades/primer-movimiento/images/verificar-guia-emitida2.png) |
