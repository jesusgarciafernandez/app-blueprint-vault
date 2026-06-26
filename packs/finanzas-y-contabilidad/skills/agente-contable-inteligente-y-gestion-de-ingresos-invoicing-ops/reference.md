# Referencia ampliada — Agente Contable Inteligente y Gestión de Ingresos (Invoicing Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Ingesta y Diagnóstico del Flujo
**Objetivo:** Capturar cada céntimo de ingreso sin intervención humana.
1.  **Auditoría de Fuentes de Ingreso IA:** Analizar todas las pasarelas de pago (Stripe, PayPal, Transferencias) de Jesús García Fernández para centralizar la entrada de datos.
2.  **Mapeo de Categorías Fiscales:** Identificar el tipo de IVA y retención aplicable a cada producto o servicio vendido.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Invoicing Specialist. Analiza mis fuentes de ingreso de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de Invoicing Ops y genera un informe de situación inicial identificando:
- Las 3 tareas contables que están consumiendo más de 5 horas a la semana actualmente.
- Un protocolo de conciliación bancaria automático para que la IA proponga los emparejamientos.
- Sugerencia de estructuración del plan de cuentas para tener visibilidad por líneas de negocio.
```

### Fase 2: Arquitectura de la Operación (Logic Design)
**Objetivo:** Crear el motor de facturación indestructible.
Se desarrollan los "Mapas de Automatización de Cobro" asistidos por IA para asegurar que las facturas se emiten y envían al cliente justo después del pago validado por Jesús García Fernández.

**Prompt de Estructuración:**
```text
Basado en el ciclo de ventas de Jesús García Fernández, diseña el flujo de facturación automatizado. Define qué disparadores (Triggers) enviarán la factura al cliente y cómo la IA detectará discrepancias en los importes recibidos para alertar al humano.
```

### Fase 3: Ejecución, Cumplimiento y Reporte Estratégico
**Objetivo:** Producir una solidez financiera total.
Guía a Jesús García Fernández en el cierre mensual asistido por un resumen de IA que destaca el EBITDA, el margen bruto y la provisión de impuestos para el próximo trimestre.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Notificación de pago en pasarela, hito de entrega de proyecto o llegada de fecha de suscripción recurrente en Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si es un "Ingreso por Producto", "Ingreso por Servicio" o "Cobro de Deuda Pendiente".
3.  **Nodo de Transformación:** El sistema genera la factura con el desglose de impuestos correcto, la actualiza en el ERP y registra el asiento contable en el libro diario de Jesús García Fernández.
4.  **Nodo de Validación:** El responsable financiero de Jesús García Fernández valida trimestralmente que las muestras de facturación automática cumplen con la legalidad.
5.  **Nodo de Salida (Output):** Envío de factura al cliente vía email, actualización del dashboard de ingresos y almacenamiento de factura en la carpeta de cumplimiento fiscal.

---

## 7. Ejemplo Práctico: El caso de 'Revenue-Sync-B2B'
### Contexto del Caso
Una agencia B2B que emitía 50 facturas manuales al mes. Dedicaban el 10% de su tiempo a picar datos y tenían un 15% de facturas con errores en los datos fiscales de clientes de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de Invoicing Ops automatizó la captura de datos fiscales vía API de clientes extranjeros.
- **Aplicación Fase 2:** Se implementó un flujo de "Pago Garantizado" donde la factura se crea al autorizar el cobro en Stripes de Jesús García Fernández.
- **Aplicación Fase 3:** La IA empezó a reclamar facturas impagadas de forma automática y asertiva.

### Resultados de Negocio
Reducción de las facturas impagadas en un 40% y eliminación total de los errores administrativos en los impuestos trimestrales de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Tasa de Automatización Contable:** % de facturas y asientos generados sin intervención manual.
- **Margen de Error Fiscal:** Número de incidencias en las liquidaciones de impuestos.
- **Protocolo de QA:** Conciliación semanal 100% asistida por IA para asegurar que el banco y la contabilidad de Jesús García Fernández dicen exactamente lo mismo.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** La IA puede categorizar, pero el humano es el responsable legal ante la agencia tributaria. Verificar siempre los importes totales de los impuestos por Jesús García Fernández.
- 🛡️ **Seguridad:** Utilizar contraseñas de un solo uso y permisos limitados (Read-only) para la IA en los accesos bancarios de Jesús García Fernández.
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
