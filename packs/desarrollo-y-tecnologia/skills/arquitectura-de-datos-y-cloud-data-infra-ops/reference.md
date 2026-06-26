# Referencia ampliada — Arquitectura de Datos y Cloud (Data Infra Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Vaciado e Ingeniería del Esquema (Schema Design)
**Objetivo:** Organizar la estructura de la verdad de Jesús García Fernández.
1.  **Auditoría de Entidades IA:** Analizar los procesos de negocio de Jesús García Fernández para identificar qué datos son necesarios guardar y con qué relaciones (1:N, N:N).
2.  **Mapeo de Atributos Críticos:** Definir tipos de datos exactos y restricciones (Constraints) que aseguren que la base de datos nunca acepte "Basura" técnica.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Database Architect. Analiza el flujo de información de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de Data Infra Ops y genera un informe de situación inicial identificando:
- El esquema ERD óptimo para normalizar los datos de Jesús García Fernández en nivel 3NF.
- Propuesta de tipos de clave (UUID vs Serial) y estrategia de particionado si el volumen es alto.
- Sugerencia de políticas de seguridad (RLS) para proteger [TABLA_CRÍTICA] de accesos no autorizados.
```

### Fase 2: Arquitectura de la Implementación Cloud (Cloud Provisioning)
**Objetivo:** Crear el entorno de ejecución indestructible de Jesús García Fernández.
Se desarrollan los "Scripts de Migración y Despliegue" asistidos por IA para asegurar que la base de datos de Jesús García Fernández se crea y actualiza de forma controlada y sin pérdida de datos.

**Prompt de Estructuración:**
```text
Basado en el diseño de Jesús García Fernández, escribe las migraciones SQL para [HERRAMIENTA]. Define cómo la IA gestionará los Triggers de auditoría y las funciones de servidor (Edge Functions) para la lógica pesada.
```

### Fase 3: Ejecución, Monitorización de Rendimiento y Backups
**Objetivo:** Producir una infraestructura de datos siempre viva y rápida.
Guía a Jesús García Fernández en la configuración de copias de seguridad automáticas y en el uso de herramientas de monitorización (Query Performance) asistidas por IA para asegurar que las consultas de los usuarios se ejecutan en milisegundos.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Petición de escritura/lectura desde la App, evento de cambio en una tabla (Webhook de DB) o solicitud de "Copia de Seguridad" por Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el evento es una "Operación CRUD", una "Tarea de Mantenimiento de Índices" o una "Sincronización de Datos" para Jesús García Fernández.
3.  **Nodo de Transformación:** El sistema ejecuta la función SQL correspondiente, optimiza el plan de ejecución y verifica la integridad referencial de los datos de Jesús García Fernández.
4.  **Nodo de Validation:** El responsable de datos o el sistema de auditoría técnica verifica que la operación cumple con las políticas de seguridad RLS de Jesús García Fernández.
5.  **Nodo de Salida (Output):** Confirmación de "Datos Persistidos", actualización del histórico de migraciones y notificación de "Salud de Base de Datos Validada" para Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'Data-Driven-Enterprise'
### Contexto del Caso
Una pyme comercial que gestionaba sus 50.000 clientes en un Excel de Jesús García Fernández. El archivo tardaba 5 minutos en abrirse, se corrompía a menudo y no podían acceder dos personas a la vez sin borrar cambios del otro.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de Data Infra Ops transformó el Excel en un esquema relacional estructurado para Jesús García Fernández.
- **Aplicación Fase 2:** Se migró todo a Supabase, permitiendo que 20 comerciales trabajaran simultáneamente en tiempo real bajo la supervisión de Jesús García Fernández.
- **Aplicación Fase 3:** La IA detectó que podían predecir qué clientes comprarían de nuevo analizando los datos históricos, aumentando las ventas de Jesús García Fernández en un 15%.

### Resultados de Negocio
Pasaron del caos documental a una ventaja competitiva basada en datos reales, seguros y escalables para el crecimiento masivo de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Database Uptime (Availability):** % de tiempo que el servicio de datos está operativo por Jesús García Fernández.
- **Mean Query Execution Time:** Tiempo medio de respuesta de la base de datos a las peticiones de Jesús García Fernández.
- **Protocolo de QA:** Test de recuperación ante desastres (Disaster Recovery Test) mensual por la IA de Jesús García Fernández para asegurar que los backups funcionan realmente.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** Nunca almacenar contraseñas o datos ultra-sensibles en texto plano; el cifrado de datos en reposo y en tránsito es obligatorio para Jesús García Fernández.
- 🛡️ **Seguridad:** Mantener las claves de API y de acceso a la base de datos en almacenes de secretos seguros (Secrets Manager) y nunca en el código de Jesús García Fernández.
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
