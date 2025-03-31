---
title: "Productos forestales"
date: 2023-10-12T11:46:47-03:00
draft: false
weight: 2
---

En el caso de tener el rol de **Administrador** en el CGL se pueden realizar las siguientes configuraciones de productos forestales que, a partir de la ampliación de funcionalidades realizadas para la versión 2, se amplió respecto de la versión anterior.

Desde el menú "Adminsitración/Productos forestales" se accede a todos los parámetros de configuración de Productos

![botón cámara](../images/menu_prod.png)

##### Unidades de medida
Esto se meantiene sin cambios, en general se trata de "gravimétricas" o "volumétricas", son difinidas por cada provincia. En las configuraciones estándar, sería TONELADA en el primer caso y METRO CUBICO en el segundo.

![botón cámara](../images/form_unidades.png)

Deben estar los parámetros TIPO_NUMERICO para seleccionar el que corresponda. Se asigna el nombre y la abreviatura. Finalemnte, se mostrará el listado que, como en los casos ya vistos, se podrá ver en detalle, editar, habilitar o deshabilitar.

##### Clases o Estados
Es el formato del producto que, en la nueva versión, adquirió más parámetros, dado la incorporación de clases transformadas. Deben estar las unidades de medida ya configuradas.

| Nivel 0                                   | Imágenes                                   |
| ----------------------------------------- | ------------------------------------------ |
| *Clases sin transformación*: Son las primeras que se deben registrar, originales de extracción, a partir de las cuales se inicia el proceso de transformación | ![botón cámara](../images/form_clase.png) |
| Luego de ingresar el nombre, se debe seleccionar la unidad de medida y el nivel de transformación quedará en 0 | ![botón cámara](../images/form_clase_0.png) |


| Nivel 1                                   | Imágenes                                   |
| ----------------------------------------- | ------------------------------------------ |
| *Clases con primer nivel de transformación*: Son las clases con un primer nivel de transformación, al seleccionarla se habilitará la selección del grado de elaboración que será entre 1 y 3 | ![botón cámara](../images/form_clase_1.png) |
| Según el grado de elaboración seleccionado, se listarán las clases origen que correspondan, con el grado menor a 1 del seleccionado | ![botón cámara](../images/form_grado_1.png) |
| Una vez asignado el nombre, la unidad de medida, nivel, grado y clase origen, si hay transformación directa, se registra el porcentaje de aprovechamiento, lo mismo si define piezas. Al final, se guarda |  ![botón cámara](../images/form_clase_1_1.png) | 


| Nivel 2                                   | Imágenes                                   |
| ----------------------------------------- | ------------------------------------------ |
| *Clases con segundo nivel de transformación*: Son las clases con el máximo nivel de transformación establecido, se habilitará la selección del grado de elaboración que será entre 3 y 5 (no podrá seleccionarse 0) | ![botón cámara](../images/form_clase_2.png) |
| Según el grado de elaboración seleccionado, se listarán las clases origen que correspondan, con el grado menor a 1 del seleccionado. Finalmente se guarda como en el nivel anterior | ![botón cámara](../images/form_clase_2_4.png) |

En todos los casos, se listan las clases y desde cada una de ellas se podrá ver el detalle, editar, habilitar y/o deshabilitar.

##### Clases de subproductos
También pueden considerarse sub clases. Definen los subproductos que se generan con la transformación dinámica. En principio habrá configurados dos:
- Costaneros
- Despuntes

![botón cámara](../images/form_subclass.png)

Primero debe seleccionarse la clase principal y después la derivada. Finalmente, el porcentaje de aprovechamiento. Hay que tener en cuenta que se pueden obtener más de una subclase por transformación:
- Si se configura 1 se le asigna el 100 %
- Si se configuran más de 1 se distribuyen el total del porcentaje

![botón cámara](../images/list_sub_clases.png)

En todos los casos, se listan las sub clases y desde cada una de ellas se podrá ver el detalle, editar, habilitar y/o deshabilitar.

##### Especies locales
Las especies locales, como el caso de las unidades de medida, son los parámetros de productos que menos cambios han tenido para la versión 2, solo se agregó la asignación del grupo de la especie para el aprovechamiento en su transformación.

Debe tenerse en cuenta que toda la estructura de Taxonomías de especies están registradas y disponibles desde un servicio, la llamada "Especie local" es solo la configuración del nombre vulgar de la especie utilizado en la provincia.

![botón cámara](../images/form_especies.png)

Una vez seleccionada la Familia se listan los Géneros y al seleccionar el género, se listan las Especies

![botón cámara](../images/form_especie_fam.png)

Finalmente se asigna el grupo de aprovechamiento y se guarda. Como en todos los casos, se listan las especies locales y desde cada una de ellas se podrá ver el detalle, editar, habilitar y/o deshabilitar.

##### Productos
Finalmente, con todo lo configurado previamente, se podrán registrar los productos forestales a gestionar.

![botón cámara](../images/form_prod.png)

- Se selecciona la especie local
- Se selecciona la clase
- Se setea la equivalencia en Kg
- Se setea la equivalencia en M3

Si el producto abona tasas, desde el botón correspondiente se accede al formulario. Deben estar las tasas previamente configuradas.

![botón cámara](../images/form_prod_tasa.png)

Se selecciona la tasa, se asigna el valor y se la guarda. Al guardar el producto se guardan las tasas también.

Como en los casos anteriores, se listan los productos registrado y desde cada una de ellos se podrá ver el detalle, editar, habilitar y/o deshabilitar.

##### Factores de transformación
Los factores de transformación están configurados y disponibles previamente para todos los CGL a partir de un estudio realizado por personal especializado. No obstante, tiene un pequeño margen de edición. Aunque en principio se recomienda no modificarlo hasta no probarlo y conocerlo bien.

Los parámetros en que se basa la transformación dinámica de productos son 3:
- El grupo de la Especie
- El nivel de desempeño del Establecimiento que ejecuta la transformación
- El grado de elaboración de la trasnformación a ejecutar

![botón cámara](../images/form_transf_grupo_esp.png)

Seleccionados el "grupo" y el "nivel", desde el botón "Ver Tabla" se mostrará la tabla correspondiente para todos los grados de elaboracón

![botón cámara](../images/tabla_transf.png)

Cada columna de la tabla se debe interpretar así:
- *Grado de elaboración*: Muestra el grado de elaboración de la transformación (de menor a mayor)
- *Transf. tptañ*: Muestra el aprovechamiento desde el grado 0 hasta el actual
- *Transf. por grado*: Muetra el aprovechamiento desde el grado anterior hasta el actual
- *Subprod. por grado*: Muestra el porcentaje de subproductos generado desde el grado anterior al actual
- *Residuos total*: Muestra el porcentaje de residuos generados desde el grado 0 al actual
- *Residuos por grado*: Muestra el porcentaje de residuos generado por grado de elaboración

Desde el botón de edición se podrá acceder a los valores de una fila que se pueden editar, el margen es pequeño

![botón cámara](../images/edit_transf.png)