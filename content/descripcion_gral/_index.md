+++
archetype = "chapter"
title = "Descripción General del sistema"
weight = 1
+++

El Sistema de Administración, Control y Verificación Forestal (SACVeFor) tiene una influencia directa en la mejora, el control del manejo forestal y la utilización de sus productos, eleva los niveles de formalidad en el sector, simplifica trámites burocráticos para productores, usuarios y consumidores, e incrementa la transparencia y el control social sobre el uso del recurso. Permite desarrollar en forma efectiva y eficiente las tareas de administración, control y verificación de la utilización y mercadeo de productos forestales, desde la aprobación y control de las actividades en el monte hasta el procesamiento, transporte y destino final de los productos, asegurando su trazabilidad e incrementando la transparencia de los procesos. 

#### Proceso gestionado
El proceso de trazabilidad de los productos está compuesto por ciclos de movimientos que ascienden en espiral mediante el agregado de valor a través de su procesamiento. El primero será denominado “Primer movimiento” y los siguientes “Removido”. Según los procedimientos administrativos de cada provincia, cada ciclo está compuesto por tres instancias principales que se describen a continuación:

##### Acreditación
Legitima la tenencia de los productos que posteriormente serán transportados. En el ciclo de Primer movimiento, la acreditación de productos la constituye la Autorización que la Autoridad Local (ALA) otorga a uno o más proponentes para la extracción de madera de uno o más predios, en forma de cupos para cada una de las especies en un formato primario determinado (rollos, trocillos, leña, etc.) Para los ciclos de Removido, la acreditación de los productos la constituye la documentación que legitime la recepción, por parte de un establecimiento, a nombre de su titular, de la materia prima para los productos que posteriormente serán transportados. 

##### Fiscalización
A partir de los relevamientos realizados con las ALAs de varias provincias, se determinó la inclusión de esta instancia de manera estandarizada aunque no en todos los casos es utilizada, en los que sí se utilizan, se aplica tanto para el ciclo de Primer movimiento como los de Removido. Consiste en una planificación previa de los productos a transportar y es utilizada principalmente para la liquidación unificada de tasas impositivas aplicadas al transporte de productos madereros. El resultado de esta instancia lo constituyen documentos con el nombre de “Guías” seguidos por distintas denominaciones o una letra determinada, según los procedimientos de cada caso. Obtienen los productos de la acreditación que corresponda según el ciclo, y quedan disponibles para la instancia siguiente.

##### Transporte
Constituye la instancia principal del ciclo e implica el transporte propiamente dicho de los productos ya acreditados y, según el caso, también fiscalizados. El resultado de esta instancia lo constituyen documentos con el nombre de “Guía” o “Remito” de transporte. Los productos serán obtenidos del saldo disponible de las Guías de fiscalización correspondientes, más allá del ciclo. Durante el período de vigencia de las guías o remitos, estos podrán ser controlados en tránsito por la autoridad que corresponda. La recepción formal de los productos transportados, por parte de su destinatario, servirá como acreditación para el inicio de un nuevo ciclo de removido, si fuera necesario.

#### Funcionalidades agregadas
Más allá de la incorporación del removido de productos que para el caso, no cambia el proceso general, se incorporaron en la Versión 2 del Sistema dos funcionalidades fundamentales:

##### Transformación dinámica de productos
A partir de un estudio profundo realizado en base a relevamientos de la gestión forestal en el Parque Chaqueño, cuando el SACVeFor todavía era un proyecto, se definieron procedimientos lo más estandarizados posibles para la realización de una ejecución dinámica de la transformación de productos.
Se configuró un "árbol" con las etapas de transformación, que se inician el el "rollo" y se van ramificando en distintos procesos de aplicación de transformación. Se establecieron 3 parámetros básicos para ejecutar la transformación, descontar residuos y generar subproductos:
###### Parámetros básicos
- *Grupo de la Especie*: A partir del aprovechamiento que la especie puede tener (de 1 a 6)
- *Nivel de desempeño*: Capacidad del establecimiento industrial (de 1 a 3)
- *Grado de elaboración*: Grado de transformación (de 0 a lo que se configure)

##### Gestión de madera decomisada
Si bien en la primera etapa de pruebas de la V2 del Sistema no está habilitada, esta funcionalidad ya está implementada y tiene por objeto, la gestión de madera decomisada por incumplimiento normativo, por parte de la ALA. El proceso se denomina gestión de "Guías públicas". Solo es removido.

#### Estructura del Sistema
El SACVeFor está estructurado en dos partes principales, que a su vez agrupan varios elementos. Cada una de las partes se describe especificamente:
- [Componentes principales](../componentes/index.html)
- [Servicios de datos comunes](../servicios/index.html)