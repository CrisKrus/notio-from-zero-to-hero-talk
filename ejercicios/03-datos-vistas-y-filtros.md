# 🗃️ 03 · Intermediate — Datos, vistas y filtros

> 🎯 Objetivo: practicar de forma autónoma lo visto en «Notion: From Zero to Hero». Crea los contenidos en tu espacio personal de pruebas, no dentro de esta página de enunciados.

## Enunciado

Crea una **base de datos real de tareas** (no una tabla simple) con propiedades, registros y varias vistas. Debe permitir responder preguntas distintas sin duplicar tareas.

## Propiedades mínimas

| Propiedad | Tipo |
| --- | --- |
| Nombre | Título |
| Estado | Estado |
| Prioridad | Selección: Alta, Media, Baja |
| Fecha límite | Fecha |
| Esfuerzo | Número |

## Registros de prueba

| Nombre | Estado | Prioridad | Esfuerzo |
| --- | --- | --- | --- |
| Preparar presentación | En curso | Alta | 3 |
| Revisar ejemplo | Pendiente | Media | 2 |
| Enviar recursos | Pendiente | Alta | 1 |
| Organizar notas | Hecho | Baja | 2 |
| Comprobar enlaces | En curso | Media | 1 |

Pon fechas próximas a, por lo menos, tres de los registros.

## Requisitos

- Crea vistas de tabla, tablero agrupado por Estado y calendario por Fecha límite.
- Crea una vista «Prioridades» que solo enseñe tareas no finalizadas con Prioridad Alta.
- Ordena una vista por Fecha límite.
- Abre una tarea y añade dentro una checklist de subtareas y un párrafo explicativo.

## Comprobación

- [ ] Las vistas muestran los mismos registros; editar en una actualiza las demás.
- [ ] El tablero agrupa por Estado y permite mover una tarea.
- [ ] El calendario representa los elementos que tienen fecha.
- [ ] «Prioridades» excluye tareas completadas y de prioridad no alta.
- [ ] La página de un registro contiene bloques, además de propiedades.

<details>
<summary>💡 Pistas</summary>

- Para una base de datos, selecciona «Tabla» como vista de base de datos, no el bloque «Tabla simple».
- Añade vistas desde el selector superior de vistas.
- El filtro avanzado combina criterios como «Estado no es Hecho» y «Prioridad es Alta».
- Una entrada de base de datos sigue siendo una página: ábrela.

</details>

<details>
<summary>✅ Solución orientativa</summary>

Una sola base «Tareas» con cinco registros, cinco propiedades y cuatro vistas: Tabla, Tablero (Estado), Calendario (Fecha límite), Prioridades (Estado distinto de Hecho y Prioridad Alta). Dentro de la tarea «Preparar presentación» hay una descripción y una checklist. Cambiar «Enviar recursos» a Hecho lo elimina automáticamente de la vista Prioridades.

</details>

## Bonus

Añade una propiedad Fórmula simple o crea una vista agrupada por Prioridad. Explica qué cambia y qué no cambia al modificar la presentación.

---

[Original en Notion](https://www.notion.so/418dacc8667981448596d45f8bb6582e) · Última edición del original: 2026-11-16.

[← Reto anterior](02-paginas-y-navegacion.md) · [Índice de ejercicios](README.md) · [Reto siguiente →](04-bases-de-datos-relacionadas.md)
