---
title: "TRAZ_PUB_ALA"
date: 2023-09-21T16:23:58-03:00
draft: false
weight: 2
---

## Configuraciones

- Personas privadas: Administración de personas que se representan a sí mismos y gestionan movimiento de productos mediante establecimientos, operando como usuarios del sistema. Estas personas son registradas previamente un servicio de datos comunes para entidades: RUE. Solo se configuran las personas privadas (Actuantes) vinculadas a Establecimientos gestionados por la ALA a la que representa el usuario.

- Establecimientos: Administración de los Establecimientos gestionados por la ALA, que se encuentran dentro de su territorio. Cada Establecimiento debe tener un Actuante como responsable, una ubicación y un nivel de desempeño. Solo se pueden configurar Establecimientos que no sean predios, estos últimos son la representación de Autorizaciones para la extracción de productos, gestionadas por la ALA y se registrarán al generar una guía de transporte de primer movimiento. Para poder ser seleccionados como origen o destino de una guía de transporte, deben estar validados y habilitados. Habrá un caso particular de Establecimientos que serán los públicos, que representan a una ALA y podrán ser seleccionados como origen de guías de transporte públicas (productos decomisados).

- Martillo para Establecimientos: Se agregó la asignación de una imagen para usar como martillo, no es obligatoria y tiene una gestión específica. Se podrá asignar y editar en Establecimientos ya registrados. En el listado se agregó el botón:

## Gestiones

- Acreditaciones: Se trata de la gestión de productos acreditados a Establecimientos, públicos y privados. Estos productos, según el caso, pueden provenir de madera decomisada (públicos) o de productos recibidos desde ALAs no vinculadas al SACVeFor (privados); por otra parte, también se podrá gestionar los remanentes de productos que queden tanto en guías como en acreditaciones externas.

- Guías: Se trata de la gestión de movimiento de productos, tanto de primer movimiento como de removido. Las funcionalidades para la gestión serán las siguientes:

  - Registrar: Se trata del registro, previo a la emisión, de guías amparan el transporte de productos.

  - Emitir: Se trata de la emisión de guías de transporte, que quedan pendientes para su recepción (cierre) por parte de sus destinatarios.

  - Editar guías emitidas: Se trata de la posible cancelación o la extensión de vigencia de una guía emitida.

  - Homologar: Se trata de la homologación de productos recibidos por Establecimientos gestionados por la ALA representada provenientes de otra provincia. Deja los productos disponibles para ser utilizados como fuente para otro movimiento originado desde el Establecimiento que los recibió.

  - Validar: Se trata de la validación de la solicitud de una guía de transporte solicitada por su titular. La dejará en condiciones de ser emitida.
