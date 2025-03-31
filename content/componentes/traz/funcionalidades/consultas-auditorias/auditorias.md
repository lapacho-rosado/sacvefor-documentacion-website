---
title: "Auditorías"
date: 2023-10-02T16:31:00-03:00
draft: false
weight: 3
---

Las auditorías pueden realizarse por usuarios con los mismos roles que las consultas:

- **TRAZ_PUB_ALA**
- **TRAZ_PRIV**
- **CONSULTA**

## Auditorías de guías

| Pasos                                                                                                                                                                                                                                                                                          | Imagen                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------- |
| En el caso de los roles **TRAZ_PUB_ALA** y **CONSULTA** permitirá el ingreso del código de guías emitidas desde establecimientos gestionados por la ALA.</br>En el caso del rol **TRAZ_PRIV**, permitirá el ingreso del código de guías emitidas desde establecimientos vinculados al usuario. | ![auditoría de guía 1](../images/auditorias-guias1.png) |
| Una vez ingresado el código, se buscan los resultados con el botón de lupa.                                                                                                                                                                                                                    |                                                         |
| Lista la guía y permite acceder desde la derecha al listado de ítems mediante el botón del ojo y al historial de cambios de la guía mediante el botón de tres barras.                                                                                                                          |                                                         |
| En el primer caso, muestra el listado de los ítems y desde cada uno permite ver el historial de cambios mediante el botón de tres barras.                                                                                                                                                      |                                                         |
| En cada caso, el historial muestra en un modal el listado con los cambios que pudo haber tenido el objeto auditado durante su gestión.                                                                                                                                                         |                                                         |

## Auditorías de acreditaciones

| Pasos                                                                                                                                                                                                                                           | Imagen                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| En el caso de los roles **TRAZ_PUB_ALA** y **CONSULTA** buscará acreditaciones asignadas a establecimientos gestionados por la ALA.</br>En el caso de **TRAZ_PRIV**, buscará acreditaciones asignadas a establecimientos vinculados al usuario. | ![auditoría de acreditaciones 1](../images/auditorias-acreditaciones1.png) |
| El ingreso del código y la búsqueda serán de la misma forma que para las auditorías de guías.                                                                                                                                                   |                                                                            |
| Los objetos retornados y los mecanismos para obtener historiales (de la acreditación y del item) son los mismos y muestran los resultados de la misma forma que en la auditoría de guías.                                                       |                                                                            |
