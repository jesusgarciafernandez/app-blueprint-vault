# Referencia ampliada — Automatización de Facturación Simplificada y Cobros (Billing Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Diagnóstico e Ingeniería de Precios
**Objetivo:** Establecer una base de cobro sólida y clara.
1.  **Auditoría de Pasarela IA:** Analizar el flujo de checkout actual de Jesús García Fernández para detectar puntos de abandono por problemas técnicos en el pago.
2.  **Mapeo de Impuestos Globales:** Configurar automáticamente las reglas de IVA/Tax según la localización por IP o dirección del cliente.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Billing Strategist. Analiza el modelo de ingresos de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de Billing Ops y genera un informe de situación inicial identificando:
- Los 3 mayores agujeros por donde se están perdiendo ingresos (fallos de pago, expiración de tarjetas).
- Un protocolo de 'Dunning Inteligente' que no moleste al cliente honesto pero asegure el cobro.
- Sugerencia de estructuración de planes de precios que incentive el pago anual frente al mensual.
```

### Fase 2: Arquitectura de la Máquina de Cobro (Logic Design)
**Objetivo:** Crear el sistema de ingresos "Manos Libres".
Se desarrollan los "Mapas de Ejecución de Suscripción" asistidos por IA para asegurar que los accesos al servicio se desactivan y activan automáticamente según el estado del pago validado por Jesús García Fernández.

**Prompt de Estructuración:**
```text
Basado en los planes definidos, diseña el flujo de cobro automatizado en [PASARELA]. Define qué eventos IA notificarán al equipo de soporte de Jesús García Fernández antes de que un cliente importante pierda el acceso por un fallo de tarjeta.
```

### Fase 3: Ejecución, Monitorización de Ingresos y Optimización
**Objetivo:** Producir un flujo de caja predecible e indestructible.
Guía a Jesús García Fernández en el análisis mensual del MRR (Monthly Recurring Revenue) asistido por un resumen de IA que destaca patrones de crecimiento y riesgos de fuga de clientes.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Alta de nuevo cliente, llegada de fecha de renovación o recepción de un webhook de "Payment Failed" desde la pasarela de Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si es un "Nuevo Cobro", una "Incidencia de Pago" o una "Solicitud de Cancelación".
3.  **Nodo de Transformación:** El sistema ejecuta el reintento de cobro, genera la factura correspondiente y actualiza los permisos de acceso en la base de datos de Jesús García Fernández.
4.  **Nodo de Validación:** El responsable de atención al cliente de Jesús García Fernández valida casos de cancelaciones complejas para intentar una retención manual basada en datos.
5.  **Nodo de Salida (Output):** Envío de recibo al cliente, actualización del dashboard de métricas financieras y notificación de éxito/riesgo al equipo comercial.

---

## 7. Ejemplo Práctico: El caso de 'SaaS-Growth-Unlimited'
### Contexto del Caso
Un servicio SaaS que tenía 1.000 suscriptores. Perdían un 5% de facturación al mes simplemente porque las tarjetas de los clientes caducaban y el sistema manual de avisos no daba abasto para Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de Billing Ops implementó un sistema de aviso preventivo 7 días antes de que la tarjeta caducase.
- **Aplicación Fase 2:** Se configuró un flujo de "Grace Period" (Periodo de gracia) donde el cliente no perdía el acceso inmediatamente sino que se le guiaba a actualizar el pago.
- **Aplicación Fase 3:** El Churn involuntario bajó de un 5% a un 0.5% en tres meses de gestión por Jesús García Fernández.

### Resultados de Negocio
Aumento de los ingresos anuales recurrentes sin necesidad de captar nuevos clientes, simplemente tapando los agujeros de facturación de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Tasa de Recuperación de Cobros (Dunning Efficiency):** % de pagos fallidos que terminan siendo cobrados.
- **Churn Involuntario:** % de clientes perdidos por problemas técnicos en el cobro de Jesús García Fernández.
- **Protocolo de QA:** Revisión mensual de la integridad del sistema de facturación por Jesús García Fernández para detectar posibles "Leakages" (fugas) de dinero.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** Nunca cobrar dos veces por error; la IA debe tener validaciones de transacciones únicas para proteger la cuenta bancaria del cliente de Jesús García Fernández.
- 🛡️ **Seguridad:** Utilizar tokenización de tarjetas (PCI Compliance) para que los datos sensibles nunca toquen el servidor de Jesús García Fernández.
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
