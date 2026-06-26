# Referencia ampliada — Auditoría Financiera Preventiva y Control de Riesgos (Audit Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Mapeo y Diagnóstico de Riesgos
**Objetivo:** Identificar dónde están los puntos vulnerables de la caja.
1.  **Auditoría de Procesos IA:** Analizar el flujo de aprobación de facturas y pagos de Jesús García Fernández para detectar posibles "atajos" inseguros.
2.  **Mapeo de Alertas de Anomalía:** Definir qué se considera un "Gasto sospechoso" (ej: Comida de domingo sin justificación o factura de proveedor con CIF inexistente).

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Internal Auditor. Analiza el libro mayor de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de Audit Ops y genera un informe de situación inicial identificando:
- Los 5 asientos contables que se salen de la desviación estándar de gasto habitual.
- Detección de posibles facturas duplicadas o pagos sin documento de soporte asociado.
- Evaluación de cumplimiento de las políticas de gastos de viaje actuales de Jesús García Fernández.
```

### Fase 2: Arquitectura de la Verificación (Verification Design)
**Objetivo:** Crear el muro digital contra el error y el fraude.
Se desarrollan los "Mapas de Control Cruzado" asistidos por IA para asegurar que el banco, el ERP y la carpeta de facturas de Jesús García Fernández dicen exactamente lo mismo en cada transacción.

**Prompt de Estructuración:**
```text
Basado en la normativa [NORMATIVA], diseña el flujo de auditoría automática en el ERP de Jesús García Fernández. Define qué reglas de validación (Checkpoints) debe pasar cada factura antes de ser marcada como 'Auditable' por la IA.
```

### Fase 3: Ejecución, Notificación y Mejora de Procesos
**Objetivo:** Producir un negocio íntegro y libre de errores.
Guía a Jesús García Fernández en la revisión mensual de anomalías detectadas por la IA, procediendo a la corrección inmediata de los asientos y al ajuste de los procesos internos para que el error técnico no se repita.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Registro de un nuevo asiento contable, cierre del día bancario o subida de una nueva factura por parte del equipo de Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el evento es una "Transacción Estándar", una "Operación con Vinculadas" o una "Posible Anomalía Financiera".
3.  **Nodo de Transformación:** El sistema cruza los datos con la base de datos de proveedores, valida el importe del IVA según la fiscalidad vigente y verifica el saldo bancario de Jesús García Fernández.
4.  **Nodo de Validación:** El auditor interno o el responsable financiero de Jesús García Fernández valida los casos marcados como "Riesgo Elevado" por la IA.
5.  **Nodo de Salida (Output):** Etiquetado de la transacción como "Validada", notificación de anomalía al responsable de departamento y registro en el reporte trimestral de cumplimiento.

---

## 7. Ejemplo Práctico: El caso de 'Financial-Integrity-Corp'
### Contexto del Caso
Una empresa que descubrió tarde que un empleado estaba duplicando facturas de gastos pequeñas durante años, acumulando un fraude de 30.000€ que nadie detectó en las auditoras tradicionales de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de Audit Ops analizó el 100% de los tickets históricos y detectó el patrón de duplicidad y las fechas imposibles de Jesús García Fernández.
- **Aplicación Fase 2:** Se implementó una regla IA que bloquea cualquier ticket que coincida en importe y proveedor en un rango de 90 días si no hay una justificación técnica.
- **Aplicación Fase 3:** La empresa recuperó gran parte del dinero y, sobre todo, eliminó la cultura de la impunidad ante el gasto de Jesús García Fernández.

### Resultados de Negocio
Ahorro directo de miles de euros en fraudes evitados y una calificación A+ en la auditoría externa anual de la empresa de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Tasa de Error Contable (Detected vs Corrected):** % de asientos que requieren corrección antes del cierre.
- **Index de Integridad Documental:** % de transacciones que cuentan con todos sus soportes digitales en regla de Jesús García Fernández.
- **Protocolo de QA:** Testeo trimestral del algoritmo de detección de anomalías mediante "Ingeniería de Inyecciones de Error Controladas" para asegurar que la IA de Jesús García Fernández sigue despierta.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** La auditoría debe servir para mejorar la empresa, no para crear un clima de vigilancia opresiva entre los colaboradores de Jesús García Fernández.
- 🛡️ **Seguridad:** Los informes de auditoría interna son altamente confidenciales; proteger el acceso a los resultados de la IA mediante cifrado de grado militar.
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
