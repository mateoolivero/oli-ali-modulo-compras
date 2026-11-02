# Backlog: historias de usuario

Cada historia está cargada como *issue* en el repositorio y vinculada al tablero de GitHub Projects, donde se sigue su estado (**Por hacer → En progreso → Listo**). Las tres historias salen de los actores del proceso BPMN ([diagramas/reposicion-oli-ali.svg](../diagramas/reposicion-oli-ali.svg)).

---

## HU-01 · Reporte de rotación para decidir compras

**Como** dueño y responsable de compras de Olí Ali,
**quiero** ver un reporte de rotación por artículo, categoría y proveedor,
**para** decidir qué y cuánto comprar con datos objetivos y no "a ojo".

**Criterios de aceptación**

- El reporte muestra las unidades vendidas y el stock actual de cada artículo, por período y por sucursal.
- Puedo filtrar por categoría, temporada y proveedor.
- La rotación se calcula en unidades, no en pesos.
- El reporte carga en menos de 3 segundos.

**Tarea BPMN asociada:** *Revisar sugerencia y reportes* (carril Dirección / Compras).
**Prioridad:** Alta · **Estimación:** 8 puntos

---

## HU-02 · Alerta de stock mínimo por sucursal

**Como** encargada de sucursal,
**quiero** recibir una alerta cuando un artículo de mi local queda por debajo del stock mínimo,
**para** verificar el stock físico y pedir la reposición antes de que se produzca el quiebre.

**Criterios de aceptación**

- La alerta indica artículo, talle, color, stock actual y stock mínimo.
- Solo veo las alertas de mi sucursal.
- Las alertas se generan con un desfase máximo de 24 horas respecto del último movimiento de stock.
- Si el stock físico no coincide, puedo marcarlo para que se ajuste en Dragonfish.

**Tareas BPMN asociadas:** *Generar alerta y sugerencia de reposición* (Módulo) y *Verificar stock físico en el local* (Encargada).
**Prioridad:** Alta · **Estimación:** 5 puntos

---

## HU-03 · Importación diaria auditable desde Dragonfish

**Como** responsable de sistemas,
**quiero** que la importación diaria de ventas y stock desde Dragonfish registre su duración y los registros rechazados,
**para** auditar que el sistema cumpla las metas de rendimiento y precisión.

**Criterios de aceptación**

- Cada corrida guarda fecha y hora, archivo de origen, duración, registros procesados, registros rechazados y estado.
- Si la importación falla, se registra el error y se avisa a Sistemas, sin cargar datos parciales.
- La importación de un día completo tarda menos de 5 minutos.

**Tareas BPMN asociadas:** *Importar ventas y stock de Dragonfish*, compuerta *¿Importación correcta?* y *Registrar error y avisar a Sistemas* (carril Módulo).
**Prioridad:** Muy alta (es requisito de HU-01 y HU-02) · **Estimación:** 5 puntos
