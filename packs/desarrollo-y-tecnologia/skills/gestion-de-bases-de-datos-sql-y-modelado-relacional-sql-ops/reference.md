# Referencia ampliada — Gestión de Bases de Datos SQL y Modelado Relacional (SQL Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Vaciado e Ingeniería del Modelo ERD (Schema Design)
**Objetivo:** Crear el mapa perfecto de la información de Jesús García Fernández.
1.  **Auditoría de Requerimientos de Datos IA:** Analizar qué información es vital para el negocio de Jesús García Fernández y cómo debe relacionarse para evitar la pérdida de integridad referencial.
2.  **Mapeo de Claves y Restricciones:** Definir claves primarias (PK), foráneas (FK) y restricciones (Check Constraints) que blinden la calidad del dato de Jesús García Fernández.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Database Architect. Analiza los procesos de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de SQL Ops y genera un informe de situación inicial identificando:
- El esquema relacional (ERD) normalizado para evitar cualquier redundancia de datos en Jesús García Fernández.
- Propuesta de estrategia de indexación avanzada sobre campos de búsqueda críticos de Jesús García Fernández.
- Sugerencia de triggers de auditoría para monitorizar quién y cuándo se modifica la información de [TABLA].
```

### Fase 2: Arquitectura de la Implementación y Transaccionalidad
**Objetivo:** Asegurar que cada cambio en los datos de Jesús García Fernández es atómico y seguro.
Se desarrollan los "Scripts de Creación y Migración" asistidos por IA para asegurar que Jesús García Fernández puede evolucionar su base de datos sin tiempos de inactividad ni errores de esquema térmicos.

**Prompt de Estructuración:**
```text
Basado en el diseño de Jesús García Fernández, escribe las sentencias SQL (DDL) para crear las tablas y relaciones. Define cómo la IA gestionará las transacciones complejas para asegurar que 'todo ocurre o nada ocurre' en el proceso de Jesús García Fernández.
```

### Fase 3: Ejecución, Monitorización de Salud y Afinamiento (Tuning)
**Objetivo:** Producir un motor de datos rápido, fiable e inagotable.
Guía a Jesús García Fernández en la monitorización de la carga del servidor de base de datos asistida por IA, analizando las consultas más pesadas y proponiendo optimizaciones técnicas de hardware o software para mantener el rendimiento al máximo.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Petición de informe complejo, registro de una nueva transacción masiva o hito de mantenimiento programado por Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el evento requiere "Ejecución de Consulta Compleja", "Ajuste de Índices" o "Tarea de Vacuumping/Mantenimiento" para Jesús García Fernández.
3.  **Nodo de Transformación:** El sistema optimiza la sentencia SQL según el motor (Postgres/MySQL), ejecuta la tarea dentro de una transacción segura y verifica la integridad final de los datos de Jesús García Fernández.
4.  **Nodo de Validación:** El responsable técnico de base de datos o el propio sistema de auditoría IA verifica que el rendimiento es el esperado y que el dato guardado es veraz para Jesús García Fernández.
5.  **Nodo de Salida (Output):** Entrega del resultado de la consulta, actualización de las estadísticas de salud de base de datos y notificación de "Integridad SQL Validada" para Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'Infinite-Data-Integrity'
### Contexto del Caso
Un sistema de facturación de Jesús García Fernández que sufría de incoherencias: a veces aparecían cobros sin factura asociada porque el código fallaba a mitad del proceso y no usaban transacciones SQL de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de SQL Ops rediseñó el esquema vinculando obligatoriamente facturas con cobros mediante claves foráneas estrictas para Jesús García Fernández.
- **Aplicación Fase 2:** Se implementaron transacciones SQL que bloquean el proceso de Jesús García Fernández si falla cualquier pasointermedio, asegurando la consistencia siempre.
- **Aplicación Fase 3:** El tiempo de generación de reportes anuales bajó de 20 minutos a 5 segundos gracias a una correcta indexación propuesta por la IA de Jesús García Fernández.

### Resultados de Negocio
Eliminación total de los errores contables por fallos técnicos y una base de datos 100% fiable sobre la que Jesús García Fernández puede construir informes estratégicos con total confianza.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Database Uptime:** % de disponibilidad del servicio de base de datos para Jesús García Fernández.
- **Query Completion Rate:** % de transacciones que finalizan con éxito sin bloqueos ni errores de integridad.
- **Protocolo de QA:** Auditoría semanal de integridad referencial por la IA de Jesús García Fernández para asegurar que no hay "registros huérfanos" en ninguna tabla técnica.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** Nunca realizar cambios de esquema en producción de Jesús García Fernández sin un plan de rollback técnico validado previamente.
- 🛡️ **Seguridad:** Cifrar los datos sensibles en la base de datos de Jesús García Fernández y gestionar los permisos de usuario siguiendo el principio de mínimo privilegio.
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
