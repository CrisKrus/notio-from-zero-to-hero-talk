# 🦸 05 · Hero — Botones, gráficos y reutilización

> 🎯 Objetivo: practicar de forma autónoma lo visto en «Notion: From Zero to Hero». Crea los contenidos en tu espacio personal de pruebas, no dentro de esta página de enunciados.

## Enunciado

Da un paso más con las bases del ejercicio anterior. Queremos ahorrar clics al crear tareas y disponer de un resumen visual del trabajo.

## Requisitos

- En tu página «Panel», crea un **botón** llamado «Nueva tarea de seguimiento».
- Configura una acción que añada un registro a «Tareas».
- Configura valores iniciales: Estado = Pendiente, Prioridad = Media; asigna un título reconocible.
- Pulsa el botón y comprueba que aparece el nuevo registro en la base real.
- Crea un gráfico de barras o anillos que muestre el número de tareas según Estado.
- Cambia el Estado de una tarea y comprueba si cambia el gráfico.
- Explica en una frase cuándo preferirías un botón y cuándo una plantilla.

> ℹ️ Los gráficos y ciertas acciones de automatización pueden variar según el plan y los permisos. En el plan gratuito puede probarse un gráfico; si ya has usado ese cupo, completa la alternativa de abajo.

## Alternativa sin gráfico disponible

Crea una vista de tablero agrupada por Estado y usa el recuento de elementos de cada grupo. Deja constancia de lo que verías en un gráfico con esos mismos datos.

## Comprobación

- [ ] El botón crea una nueva tarea en la base correcta.
- [ ] La tarea creada contiene los valores por defecto previstos.
- [ ] Puedo distinguir la vista visual de los datos de origen.
- [ ] Sé justificar cuándo reutilizar una plantilla y cuándo ejecutar un botón.

<details>
<summary>💡 Pistas</summary>

- Busca el bloque «Botón» con `/`.
- Entre las acciones de botones, busca «Añadir página a» y selecciona la base Tareas.
- Para gráficos, añade una vista del tipo Gráfico a la base de datos y selecciona agrupación por Estado.
- Para revisar las acciones disponibles y sus límites, consulta [la ayuda de botones](https://www.notion.com/help/database-buttons) y [la ayuda de gráficos](https://www.notion.com/help/charts).

</details>

<details>
<summary>✅ Solución orientativa</summary>

El Panel contiene un botón que añade a Tareas la entrada «Revisar seguimiento», con estado Pendiente y prioridad Media. La vista Gráfico agrupa por Estado (o, en la alternativa, un tablero muestra el recuento por columna). Una plantilla prepara el contenido interno de una página; un botón ejecuta acciones al pulsarlo. Se pueden combinar.

</details>

## Bonus opcional

Explora un botón de propiedad dentro de la base de datos que cambie el Estado de la tarea actual. No necesitas utilizar integraciones externas ni Notion AI.

---

[Original en Notion](https://www.notion.so/418dacc86679810596d9cc7815e1b0b9) · Última edición del original: 2026-11-16.

[← Reto anterior](04-bases-de-datos-relacionadas.md) · [Índice de ejercicios](README.md)
