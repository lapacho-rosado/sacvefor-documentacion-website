---
title: "Acceso usuarios registrado"
date: 2023-10-20T10:44:08-03:00
draft: false
weight: 2
---

El acceso para uuarios registrados al CTRL permite consultar la validez de una guía o remito durante su ciclo de vida mediante una consulta
según las siguientes opciones:

- Matrícula de vehículo
- Código de la Guía o remito
- CUIT del Remitente de la Guía o remito
- Entidad origen del movimiento
- CUIT del Destinatario de la Guía o remito
- Entidad destino del movimiento


En prioncipio, dede la administración hay configurado un usuario de acceso para mostrar las funcionalidades. Desde la aplicación se debe acceder al formulario de inicio de sesión:

![botón cámara](../images/inicio_sesion.png)

Se ingresarán los datos estándar:
- 14008000
- 1234

![botón cámara](../images/form_inicio.png)

Una vez inicia la sesión se mostrará la pantalla del usuario:

![botón cámara](../images/incio_con_sesion.png)

Lo más importante, por ahora es la descripción de las diferentes consultas cuyo acceso muestra la barra inferior

| Pasos                     | Imágenes                                |
| ------------------------- | --------------------------------------- |
| **Matricula**, al acceder se muestra un listado como en el caso de la consulta pública, con el agregado de los detalles | ![botón cámara](../images/detalles_por_matricula.png) |
| *Vehículo* muetra el detalle del transporte | ![botón cámara](../images/detalle_transporte.png) |
| *Detalle Origen* muetra el detalle del origen de los productos | ![botón cámara](../images/detalle_origen.png) |
| *Detalle Destino* muetra el detalle del destino de los productos | ![botón cámara](../images/destino_prod.png) |
| *Detalle Fuente de productos* muetra el listado de las guía base fuentes de los productos | ![botón cámara](../images/detalle_fuentes.png) |
| *Detalle de Productos* muetra el detalle de los productos transportados | ![botón cámara](../images/detalle_prod.png) |
| Desde el nombre vulgar se puede acceder a más información que pudiera haber | ![botón cámara](../images/mas_detalle_prod.png) |
| Las consultas por **Código**, **CUIT de Remitente**, **Entidad Origen**, **CUIT Destinatario** y **Entidad Destino**, retornan todos la misma estructura de información, con la diferencia de que el listado puede contener más o menos guías, dado que los parámetros de búsqueda son más o menos genéricos. Desde los botones de la derecha se accede a la informacióon ya detallada | ![botón cámara](../images/listado_generico.png) |
