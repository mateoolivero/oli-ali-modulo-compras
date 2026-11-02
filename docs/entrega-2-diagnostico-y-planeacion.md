# Entrega 2 · Diagnóstico y planeación del proyecto tecnológico

## FODA del proyecto

| | Positivo | Negativo |
|---|---|---|
| **Interno** | **Fortalezas:** conocimiento del negocio desde adentro; acceso directo al dueño; manejo de JavaScript/React, Next.js, Supabase y Python; bajo costo de desarrollo | **Debilidades:** equipo unipersonal; sin experiencia previa en análisis de datos; desconocimiento técnico de lo que exporta Dragonfish; sin entorno de pruebas formal |
| **Externo** | **Oportunidades:** voluntad del dueño de profesionalizar; necesidad inmediata (compras "a ojo"); expansión a sucursales; posibilidad de replicarlo en otras tiendas con Dragonfish | **Amenazas:** dependencia de un sistema de terceros; inflación; resistencia al cambio; temporada alta |

**Estrategias:** indicadores pensados para decisiones de compra reales; base de datos multisucursal desde el inicio; desarrollo incremental; involucrar al dueño y a las encargadas desde el relevamiento; medir en unidades y no en pesos; aislar la importación de Dragonfish en un módulo independiente.

## Objetivo general

Desarrollar e implementar, entre octubre de 2026 y febrero de 2027, un módulo de análisis y reportes alimentado por los datos de ventas y stock de Dragonfish, para que las compras a proveedores de Olí Ali se basen en indicadores objetivos de rotación, estacionalidad, quiebres de stock y rendimiento por proveedor.

## Metas cuantitativas

| Meta | Estándar |
|---|---|
| Rendimiento | Importación diaria en menos de 5 minutos; reportes en menos de 3 segundos |
| Escalabilidad | 3 años de histórico (hasta 500.000 líneas de venta) y **al menos 6 sucursales** sin rediseño *(actualizada en la Entrega 3: originalmente eran 3)* |
| Precisión | Coincidencia ≥ 99,5 % con Dragonfish |
| Oportunidad | Alertas de stock mínimo con desfase máximo de 24 horas |
| Plazo | En producción antes del 5 de febrero de 2027 |

## Planificación (Gantt)

Inicio: 13/10/2026. Fases: Análisis → Diseño → Codificación → (pausa por temporada alta) → Pruebas → Implementación, con hitos de validación con el dueño. El diagrama completo está en el PDF consolidado.
