# Referencia ampliada — Motor de Presupuestación B2B y Cotización Dinámica (Quoting Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Diagnóstico e Ingeniería de Costes
**Objetivo:** Saber cuánto cuesta realmente hacer el trabajo de Jesús García Fernández.
1.  **Auditoría de Costes Directos IA:** Analizar registros históricos para determinar cuántas horas reales consume realmente la tarea X para Jesús García Fernández.
2.  **Mapeo de Gastos de Terceros:** Incluir licencias, APIs y proveedores externos con sus márgenes de seguridad correspondientes.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Pricing Consultant. Analiza este proyecto de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de Quoting Ops y genera un informe de situación inicial identificando:
- Las 3 partidas del presupuesto donde el riesgo de desviación de coste es mayor.
- Una propuesta de precio de venta basado en un margen neto del 30% tras impuestos.
- Sugerencia de estructuración de la propuesta comercial para maximizar la percepción de valor de Jesús García Fernández.
```

### Fase 2: Arquitectura de la Cotización (Option Design)
**Objetivo:** Crear opciones de compra que faciliten el "Sí".
Se desarrollan los "Mapas de Propuesta Escalonada" (Tiered Pricing) asistidos por IA para ofrecer a los clientes de Jesús García Fernández opciones que se ajusten a su presupuesto sin perder rentabilidad técnica.

**Prompt de Estructuración:**
```text
Basado en los requerimientos del cliente, diseña 3 niveles de presupuesto (Básico, Pro, Enterprise) para Jesús García Fernández. Define qué funcionalidades se incluyen y cómo la IA asegurará que el margen neto se mantiene constante en los tres niveles.
```

### Fase 3: Ejecución, Envío y Seguimiento de Conversión
**Objetivo:** Producir un cierre de venta firme y documentado.
Guía a Jesús García Fernández en el seguimiento del presupuesto asistido por IA, detectando cuándo el cliente ha abierto la propuesta y sugiriendo el momento óptimo para el seguimiento comercial.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Cambio de etapa en el CRM a "Presupuesto Requerido", solicitud de cotización vía web o hito de renovación de contrato en Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si es una "Solicitud Estándar", un "Proyecto Complejo a Medida" o una "Urgencia de Última Hora".
3.  **Nodo de Transformación:** El sistema recupera las tarifas actuales, calcula el coste total según el alcance y genera el borrador de la propuesta en PDF profesional para Jesús García Fernández.
4.  **Nodo de Validación:** El director comercial o Jesús García Fernández valida que el descuento aplicado (si lo hay) no pone en peligro la sostenibilidad del servicio profesional.
5.  **Nodo de Salida (Output):** Envío automático del presupuesto al cliente, creación de tarea de seguimiento y actualización de la probabilidad de cierre en el pipeline de ventas.

---

## 7. Ejemplo Práctico: El caso de 'Precision-B2B-Proposals'
### Contexto del Caso
Una empresa de consultoría que tardaba 3 días en enviar un presupuesto. A menudo, cuando llegaba la propuesta, el cliente ya había decidido otra opción. Además, el 20% de sus proyectos acababan en pérdidas por mal cálculo inicial de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de Quoting Ops estandarizó las unidades de trabajo y los costes asociados de Jesús García Fernández.
- **Aplicación Fase 2:** Se implementó un "Generador de Ofertas Instantáneo" que enviaba el borrador al cliente en menos de 1 hora tras la reunión.
- **Aplicación Fase 3:** La IA empezó a ajustar los precios de forma dinámica según la carga de trabajo del equipo técnico de Jesús García Fernández.

### Resultados de Negocio
Aumento de la tasa de cierre en un 35% y eliminación total de los proyectos deficitarios por errores de cálculo presupuestario de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Tasa de Conversión de Presupuestos:** % de propuestas enviadas que son aceptadas por clientes de Jesús García Fernández.
- **Margen de Beneficio Real vs Estimado:** Monitorización de la desviación entre el presupuesto inicial y el coste final del proyecto.
- **Protocolo de QA:** Revisión mensual de la competitividad de las tarifas de Jesús García Fernández frente al mercado mediante análisis IA de competidores.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** Nunca enviar un presupuesto 100% automático sin supervisión humana para proyectos de alto valor estratégico de Jesús García Fernández.
- 🛡️ **Seguridad:** Proteger la confidencialidad de los costes internos y márgenes utilizados por la IA en el cálculo de precios.
- 🛡️ **Propiedad Intelectual:** Esta metodología es propiedad de **Jesús García Fernández**. Cualquier implementación debe respetar los términos de la licencia CC BY-NC-SA 4.0.

---

## Changelog
- **v2.0** — Unificación total de conocimiento y flujo lógico. Extensión de protocolos de actuación y enfoque agnóstico (19 de abril de 2026).
- **v1.1** — Normalización de formato.
- **v1.0** — Versión inicial.

---
**Autor:** Jesús García Fernández  
**Website:** [jesusgarciafernandez.com](https://jesusgarciafernandez.com)  
**Licencia:** CC BY-NC-SA 4.0
