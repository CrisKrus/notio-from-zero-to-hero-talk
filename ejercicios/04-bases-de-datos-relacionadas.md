# 🔗 04 · Advanced — Bases de datos relacionadas

> 🎯 Objetivo: practicar de forma autónoma lo visto en «Notion: From Zero to Hero». Crea los contenidos en tu espacio personal de pruebas, no dentro de esta página de enunciados.

## Enunciado

Amplía el ejercicio anterior con una segunda base llamada **Proyectos**. Tu misión es conectar datos sin duplicarlos y crear una portada para consultarlos.

## Datos para Proyectos

| Nombre | Estado |
| --- | --- |
| Charla Notion | En marcha |
| Wiki del equipo | Planificado |

## Requisitos

- Crea una base de datos «Proyectos» con propiedades Nombre y Estado.
- En «Tareas», crea una propiedad de tipo **Relación** hacia «Proyectos».
- Relaciona «Preparar presentación», «Revisar ejemplo» y «Enviar recursos» con «Charla Notion».
- Relaciona «Organizar notas» con «Wiki del equipo».
- Crea una página «Panel» y añade una **vista vinculada** de «Tareas».
- Filtra esa vista para ver únicamente las tareas de «Charla Notion».
- Crea una plantilla de nueva página en «Proyectos» con secciones «Objetivo», «Próximos pasos» y «Riesgos».

## Comprobación

- [ ] Desde un proyecto puedo identificar sus tareas relacionadas.
- [ ] Si cambio una tarea en el Panel, también cambia en la base de datos original.
- [ ] En el Panel no he creado una copia independiente de Tareas.
- [ ] Una nueva entrada creada con la plantilla contiene las tres secciones.

<details>
<summary>💡 Pistas</summary>

- La propiedad «Relación» es la que conecta dos bases de datos.
- La vista vinculada se crea desde una página apuntando a una base de datos que ya existe.
- Las plantillas de una base de datos se crean en el menú del botón Nuevo de esa base.
- Un rollup puede contar tareas relacionadas, pero no es obligatorio.

</details>

<details>
<summary>✅ Solución orientativa</summary>

Existen las bases «Tareas» y «Proyectos». La relación de Tareas apunta a Proyectos y los registros quedan asignados. El Panel muestra una vista vinculada filtrada por «Charla Notion». La base original y la vista vinculada comparten registros. La plantilla de Proyectos incluye los tres encabezados reutilizables.

</details>

## Bonus

Añade un rollup que cuente tareas relacionadas por proyecto y una segunda vista en Panel con tareas pendientes de todos los proyectos.

---

[Original en Notion](https://www.notion.so/418dacc866798137898fc4c2f13c62b2) · Última edición del original: 2026-11-16.

[← Reto anterior](03-datos-vistas-y-filtros.md) · [Índice de ejercicios](README.md) · [Reto siguiente →](05-botones-graficos-y-reutilizacion.md)
