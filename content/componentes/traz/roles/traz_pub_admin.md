---
title: "TRAZ_PUB_ADMIN"
date: 2023-09-21T16:23:58-03:00
draft: false
weight: 1
---

Se trata del rol de Administrador de la aplicación. Representa a la Autoridad Nacional y tiene la responsabilidad de administrar los parámetros genéricos y específicos de la aplicación. Por estas características, las funcionalidades ejecutadas por este rol no forman parte del plan de pruebas. Tales funcionalidades se resumen a continuación:

## Administración

- Tipos de paramétricas: Administración de objetos genéricos que definen el tipo de parámetros generales a configurar, como pueden ser roles de usuario, tipos de fuentes de productos, tipos de destino de productos, tipos de movimiento, etc.

- Entidades paramétricas: Administración de parámetros generales requeridos por los distintos objetos gestionados, que definen los casos específicos de los tipos descriptos arriba.

- Estados de guía: Administración de los distintos estados por los que pasa una guía durante su ciclo de vida.

- Copias de guía: Administración de las copias que se incluyen por cada tipo de guía en el archivo PDF que se genera en su emisión.

- Tipos de guía: Administración de los distintos tipos de guías de transporte que cada provincia podrá gestionar, definidos fundamentalmente por el tipo de destino, tipo de movimiento, período de vigencia, y otras características. Se incluye en esta administración la configuración de tasas a liquidar, en el caso en que el tipo de guía liquide tasas.

## Componentes locales

Administración de los distintos Componentes de gestión local del SACVeFor (CGL) que estén vinculados a TRAZ. Cada componente local representa a la Autoridad local de una Provincia y genéricamente se lo denomina ALA. Puede haber tres tipos diferentes de vinculación:

- Vinculación completa: Se trata de Componentes locales cuya gestión mediante el CGL correspondiente está completamente vinculada con TRAZ: acceden mediante servicios a fuentes de productos, Actuantes y Establecimientos vinculados, para la gestión de Autorizaciones y guías base.

- Emisión remota: Se trata de Componentes locales vinculados a TRAZ mediante la emisión remota de guías de transporte, desde aplicaciones locales propias a través de servicios de integración de información.

- No vinculados: Se trata de Autoridades locales cuya gestión, aún no está vinculada al SACVeFor, solo están registrados para ser seleccionados como provincia de origen para la Acreditación de productos recibidos mediante guías originadas por dichas provincias.

## Personas públicas

Administración de las personas que representan a la Autoridad nacional (ANA) y a las Autoridades locales (ALA) que tendrán un usuario asignado con el rol que corresponda. Estas personas solo se registran aquí.

## Usuarios

Administración de los usuarios que podrán acceder a TRAZ para operar. Se trata de usuarios que representan a personas y usuarios que representan a otros componentes del SACVeFor.

## Acreditaciones

Edición de Acreditaciones externas a pedido de Autoridades locales, para casos que su estado no permita la edición a usuarios con que las representan.

## Consultas estado general

Desde la vista de inicio, el usuario con este rol podrá ver un estado general de las entidades administradas. Además podrá ver los Establecimientos, las personas privadas registrados.
