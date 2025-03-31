+++
archetype = "chapter"
title = "Registro de cambios"
[_build]
    render = "always"
    list = "never"
    publishResources = true
+++
## Índice
1. [CGL](#cgl)
1. [TRAZ-Backend](#traz---backend)
1. [TRAZ-Frontend](#traz---frontend)

---

## CGL
### 2.4.0 (13/12/2023)
 - Se agregó un servicio para retornar la ruta del martillo de obrajero.
### 2.3.0
 - Se ampliaron las funcionalidades de la transformación en Guías de Removido, incorporando la transformación directa.
### 2.2.0
 - Agregadas funcionalidades para mejorar la persistencia de imágenes de martillos.
### 2.1.2
 - Corregidas rutas imágenes de martillos de establecimientos.
### 2.1.1
 - Agregada vista histórica de guías emitidas.

---

## TRAZ - Backend
### 2.3.1 (13/12/2023)
 - Mejora del código para facilitar la generación de reportes de guías emitidas.
### 2.3.0
 - Se agregaron los servicios de consultas de guías en proceso, previo a la emisión, según varios roles de usuario.
### 2.1.3
 - Solucionado problema en la base de datos donde los ID de ciertas entidades figuraban duplicados, impidiendo el guardado de nuevas guías.
### 2.1.2
 - Solucionado error que impedía el inicio de sesión.
### 2.1.1
 - Corregidas estadísticas erróneas de guías y acreditaciones en el dashboard de inicio. El mismo no registraba correctamente las guías y acreditaciones generadas el mismo día.
 - Agregado CUIT faltante a la serialización del componente local y las auditorías.
 - Agregada búsqueda de componente local por CUIT a la API.
 - Se agregaron los servicios para consultar guías registradas por CUIT desde el CGL.
 - Se agregó el guardado y persistencia de archivos de imágenes para los martillos de establecimientos.

---

## TRAZ - Frontend
### 2.3.2 (13/12/2023)
Se realizaron múltiples mejoras al código para facilitar la creación de reportes de guías emitidas.
 - Se corrigieron las plantillas de reportes para que muestren correctamente el nombre de la copia y su destinatario.
 - Se corrigió la impresión de números de rodales en los reportes.
 - Se crearon directorios exclusivos para los recursos subidos de cada provincia, evitando duplicaciones.
 - Se unificaron los directorios de recursos con CGL, facilitando el acceso a recursos compartidos.
 - Se creó un servicio para consultar desde CGL la ruta de archivo de los martillos de obrajeros de una guía de primer movimiento para el caso de Misiones.
 - Se corrigió la obtención de autorizaciones de la guía desde el CGL.
 - Se agregó una línea de cierre a los ítems impresos en los reportes.
 - Se corrigió la creación de páginas de reporte según la cantidad de copias de la guía.
 - Agregada sustitución de archivos por defecto "sin martillo" en caso de que el archivo del martillo referenciado no se encuentre correctamente almacenado o no haya sido provisto por el usuario.
 - Corregido mensaje del último paso del wizard de emisión de guía, "Imprimir remito PDF".
 - Agregadas comprobaciones varias para evitar la aparición de errores al generar reportes.
### 2.3.1
 - Se corrigió un error en la llamada a la vista de personas públicas.
### 2.3.0
 - Se agregaron consultas por guías al proceso previo de la emisión, desde distintos roles de usuarios.
 - Se implementó la habilitación de gestión de usuario de TRAZ\_PUB\_ALA, sólo desde TRAZ\_PUB\_ALA y TRAZ_PRIV.
 - Se implementó la gestión de personas públicas desde TRAZ\_PUB\_ALA.
### 2.2.1
 - Renombradas "guías" a "remito" en la interfaz de usuario para implementar la terminología ya usada.
### 2.2.0
 - Agregada generación de reportes para la provincia de Corrientes.
### 2.1.3
 - Se corrigió el guardado de imágenes de martillos del establecimiento de una guía.
 - Agregados parámetros faltantes a los reportes PDF de Jujuy.
### 2.1.2
 - Se corrigió el enmascarado de la matrícula de vehículos.
 - Se corrigió el filtrado de establecimientos por CUIT en el menú de registro de guías.
 - Se corrigieron las rutas de guardado de martillos de establecimientos.
### 2.1.1
 - Se corrigió la recuperación de parámetros de filtrado al retornar desde el wizard de emisión de guía.
### 2.1.0
 - Se implementó el filtrado por CUIT en el menú de registro de guías.
 - Se simplificaron los códigos de guías generados tras la emisión.
 - Se inhabilitó el botón de cierre directo de una guía para evitar cierres accidentales.
 - Se implementó, durante la emisión de guías, la creación del usuario destinatario de una guía si es que no existe.
 - Se implementó una confirmación al emitir una solicitud de guía, desde el usuario titular.
 - Se agregaron máscaras a las matrículas de los vehículos.
 - Se ensancharon los modales que listan ítems fuentes.
