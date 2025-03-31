# README

## Descripción

Repositorio de la página web de documentación de usuarios de SACVeFor. Rama develop

El proyecto se basa en el framework [HUGO](https://gohugo.io/) que permite crear páginas web estáticas utilizando [plantillas](https://themes.gohugo.io/), de forma ágil y sencilla.

Se utiliza Docker para crear un contenedor donde automáticamente se renderiza la página y se ubica dentro de un servidor NGINX, sin requerir ninguna intervención del desarrollador.

## Comienzo rápido

### Servidor local de prueba

Una vez clonado el repositorio, se puede levantar un servidor local de prueba con la página web montada utilizando el comando `hugo serve`.  
Este servidor de prueba tiene recarga rápida, por lo que al modificar el contenido del sitio web, ya sea al modificar su ruta de archivos, agregar recursos estáticos como imágenes o videos, o modificar un archivo markdown, los cambios se verán reflejados instantáneamente.

### Opciones extra para el servidor

Si es necesario cambiar el puerto que utiliza el servidor de prueba por defecto (:1313) se puede utilizar la opción "-p [puerto]"  
`hugo server -p 8889`

Si se quiere visualizar contenido que tienen la propiedad de borradores (draft) activada, se puede usar la opción "-D"
`hugo server -D`

---

## Estructura de archivos

HUGO genera automáticamente al iniciar un proyecto una [estructura de carpetas predefinida](https://gohugo.io/getting-started/directory-structure/).  
Nuestro mayor interés estará en la carpeta "content".

El formato de archivos que trabaja HUGO es HTML y Markdown.  
Por su simplicidad, se considera mejor práctica utilizar siempre Markdown, excepto en situaciones donde no se puedan lograr los resultados deseados (Por ej: Al querer introducir listas de ítems dentro de una fila de una tabla. En ese caso se debe crear la tabla usando sintaxis markdown, pero luego utilizar sintaxis HTML para el listado de ítems dentro de la fila correspondiente).

### Carpeta "content"

Tal como indica su nombre, en esta carpeta irá la mayoría de nuestro contenido. Su estructura de archivos y carpetas reflejará la estructura que tendrá nuestro sitio web.

Ej: El archivo "\_index.md" situado en la raíz de la carpeta "content", tendrá el contenido de la homepage del sitio. Las carpetas "roles" y "funcionalidades" contendrán los archivos correspondientes de cada sección (la primera destinada a explicar roles de usuario y la segunda destinada a explicar funcionalidades para las pruebas de CGL y TRAZ).

#### URIs

El nombre de las carpetas y los archivos markdown definirán el nombre de las URI que tendrá la página.

Ej: si tenemos la ruta "content/funcionalidades/primer-movimiento/registro-de-guia-primer-movimiento.md" el enlace en la página será "localhost:1313/content/funcionalidades/primer-movimiento/registro-de-guia-primer-movimiento/index.html"

Por este motivo, conviene utilizar nombres de carpetas y archivos descriptivos, pero acotados.

#### Referencias internas

También se debe tener en cuenta que mucha documentación probablemente tendrá hipervínculos hacia secciones internas de la página.

Para eso se toma como punto de partida la raíz de la carpeta "content" y luego se sigue la ruta hasta el archivo markdown que se desea enlazar. Para finalizar, a esa ruta se le agrega una barra y luego "index.html".

Ej: Si en un artículo queremos enlazar el artículo de _asignación de productos a una asignación de remanentes_ se deberá utilizar el siguiente hipervínculo:  
`[texto del hipervínculo](/funcionalidades/remanentes/asignacion-productos/index.html)`

## Cómo agregar contenido

### Secciones

Una sección contiene varios artículos dentro de ella.

La idea actual para el contenido de las secciones es realizar diagramas de flujo que muestren cómo se van sucediendo las funcionalidades para comenzar y terminar el ciclo de una guía, así como ofrecer una breve descripción que le sea pertinente a todas las funcionalidades que contiene.

Para crear una nueva sección se puede utilizar el comando:  
`hugo new --kind chapter [ruta]/_index.md`, donde "[ruta]" corresponde a la estructura de carpetas. Si en esa ruta hay carpetas que aún no existen, HUGO las creará automáticamente.

Tener en cuenta que se debe agregar "\_index.md" al final de la ruta, ya que de lo contrario no se detectará como una sección en el renderizado de la página.

#### Encabezado de sección

Las secciones tendrán encabezados como el siguiente:

```markdown
+++
archetype = "chapter"
title = "Gestión de acreditación de remanentes"
weight = 4
+++

Acá va el contenido en markdown
```

Al utilizar el comando de arriba, HUGO lo genera automáticamente.

A nosotros nos interesa modificar "title" que será el título de la sección a mostrarse tanto en su landing page como en el menú lateral.

Luego está "weight", que determina el orden en el que se posicionará en el menú lateral en relación a las secciones ubicadas bajo la misma carpeta raíz.

Ej: Tenemos /content/funcionalidades/ y ahí varias carpetas correspondientes a secciones como "removido" o "primer-movimiento". Dentro de cada una de esas subcarpetas habrá un archivo "\_index.md" correspondiente a la landing page de la sección. Si el "weight" del encabezado dentro de "\_index.md" correspondiente a la carpeta "removido" tiene valor "1" y el mismo parámetro en la carpeta de "primer-movimiento" tiene valor "2"; la sección de Removido se listará primera en relación a la sección de Primer Movimiento que se listará segunda.

### Artículos

Los artículos corresponden a las páginas con contenido detallado de una funcionalidad y están dentro de alguna sección.

De forma parecida a la [creación de secciones](#secciones), podemos utilizar el comando:  
`hugo new [ruta]/[nombre-de-articulo].md`, donde "[ruta]" corresponde a la estructura de carpetas. Si en esa ruta hay carpetas que aún no existen, HUGO las creará automáticamente.

#### Encabezado de artículo

Los artículos tendrán encabezados [similares a los de las secciones](#encabezado-de-sección).

```markdown
---
title: "Agregar imagen de martillo de establecimiento"
date: 2023-09-21T16:46:13-03:00
draft: false
weight: 3
---

Acá va el contenido en markdown
```

Los parámetros a modificar son:

- title: Será el título que se mostrará en el encabezado del artículo al visualizarlo en la página.
- date: La fecha de creación del artículo. No se mostrará en la página.
- draft: Tendrá valor "true" o "false". Indica si el artículo está en fase de borrador o no. Los artículos borradores no se incorporarán a la versión final de la página, pero permiten trabajar en artículos estipulados para ser lanzados en una versión posterior de la página.
- weight: Tal como en las secciones, determina el posicionamiento del artículo en el menú lateral de la página, en relación al resto de los artículos dentro de la misma sección.

## Recursos adicionales

[Relearn Theme](https://mcshelby.github.io/hugo-theme-relearn/index.html): Página web de la plantilla que se utilizó para la página. Contiene información útil sobre funcionalidades propias de la plantilla, así como un [resumen de la sintaxis markdown](https://mcshelby.github.io/hugo-theme-relearn/cont/markdown/index.html).
