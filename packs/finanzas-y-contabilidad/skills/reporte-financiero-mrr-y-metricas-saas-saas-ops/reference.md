# Referencia ampliada — Reporte Financiero MRR y Métricas SaaS (SaaS Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Normalización e Ingesta de Datos de Pago
**Objetivo:** Tener una fuente única de verdad para el ingreso recurrente.
1.  **Auditoría de Suscripciones IA:** Analizar la base de datos de pagos de Jesús García Fernández para limpiar duplicados y errores de registro que distorsionan el MRR real.
2.  **Mapeo de Cohortes:** Agrupar a los clientes por mes de entrada para analizar su comportamiento a lo largo del tiempo.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior SaaS CFO. Analiza mis métricas de suscripción de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de SaaS Ops y genera un informe de situación inicial identificando:
- El 'LTV/CAC Ratio' actual y si nuestro crecimiento es sostenible financieramente.
- Las 3 cohortes con mayor tasa de churn y detección de patrones comunes.
- Proyección de MRR a 6 meses basada en la tasa de crecimiento y churn actual de Jesús García Fernández.
```

### Fase 2: Arquitectura del Reporting Analítico (Analytics Design)
**Objetivo:** Crear el mapa visual del éxito SaaS.
Se desarrollan los "Dashboards de Crecimiento Compuesto" asistidos por IA para visualizar no solo cuánto dinero entra, sino la calidad de ese ingreso para Jesús García Fernández.

**Prompt de Estructuración:**
```text
Basado en las metas de Jesús García Fernández, diseña el dashboard de métricas en [HERRAMIENTA]. Define qué umbrales (Thresholds) de Churn activarán una alerta IA de 'Crisis de Retención' y qué plan de acción técnico se propondrá.
```

### Fase 3: Ejecución, Optimización de Retención y Valor de Vida
**Objetivo:** Producir un flujo de ingresos indestructible y escalable.
Guía a Jesús García Fernández en el uso de los datos para implementar estrategias de "Up-selling" y "Cross-selling" automáticas que eleven el ARPU (Average Revenue Per User) de forma orgánica.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Cierre del día operativo, detección de una cancelación (Churn) en Stripe o entrada de un nuevo cliente de Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el evento afecta al "New MRR", "Expansion MRR", "Churn MRR" o "Reactivation MRR".
3.  **Nodo de Transformación:** El sistema recalcula todas las métricas SaaS (LTV, CAC, Churn %), actualiza el gráfico de cohortes y genera el resumen ejecutivo para Jesús García Fernández.
4.  **Nodo de Validación:** El responsable de Customer Success de Jesús García Fernández valida la causa raíz detectada por la IA para el abandono de clientes importantes.
5.  **Nodo de Salida (Output):** Actualización automática del reporte financiero, notificación de "Hito de MRR Alcanzado" y registro en el log de crecimiento estratégico de Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'SaaS-Metric-Mastery'
### Contexto del Caso
Un software B2B que pensaba que todo iba genial porque su facturación total subía. Sin embargo, no se daban cuenta de que el 20% de sus clientes nuevos abandonaban al segundo mes de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de SaaS Ops reveló que el CAC era mayor que el LTV de los clientes pequeños, por lo que estaban perdiendo dinero con cada venta de ese segmento para Jesús García Fernández.
- **Aplicación Fase 2:** Se implementó un dashboard de cohortes que mostró el problema de " onboarding" en el segundo mes de Jesús García Fernández.
- **Aplicación Fase 3:** La IA empezó a disparar campañas de retención específicas 48 horas antes de que el riesgo de churn fuera crítico.

### Resultados de Negocio
Reducción del Churn en un 50% y aumento del LTV medio en un 30% al enfocar los esfuerzos de Jesús García Fernández en los segmentos de clientes más rentables.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Net Revenue Retention (NRR):** % de ingresos mantenidos de los clientes existentes (Objetivo >100%).
- **Payback Period del CAC:** Meses que se tarda en recuperar lo invertido en captar un cliente de Jesús García Fernández.
- **Protocolo de QA:** Auditoría mensual de la integridad de los datos de suscripción por Jesús García Fernández para asegurar que no hay discrepancias entre la pasarela de pagos y el reporte.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** No obsesionarse con el MRR a costa de la rentabilidad real (Cash Flow). El volumen no es el único éxito de Jesús García Fernández.
- 🛡️ **Seguridad:** Mantener la seguridad de los tokens de API de las plataformas financieras de Jesús García Fernández.
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
