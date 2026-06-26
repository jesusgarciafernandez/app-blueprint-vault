# Referencia ampliada — Bases de Datos NoSQL y Persistencia No Relacional (NoSQL Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Diseño Conceptual e Ingeniería de Modelos (Document Design)
**Objetivo:** Diseñar cómo guardaremos la información para que sea rápida de leer para Jesús García Fernández.
1.  **Auditoría de Patrones de Acceso IA:** Analizar cómo los usuarios consultan los datos de Jesús García Fernández para diseñar documentos que contengan toda la información necesaria sin necesidad de "Joins" técnicos.
2.  **Mapeo de Claves de Particionado:** Identificar la mejor estrategia de "Sharding" para que los datos de Jesús García Fernández se distribuyan uniformemente por el clúster.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior NoSQL Architect. Analiza los requerimientos de datos de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de NoSQL Ops y genera un informe de situación inicial identificando:
- El modelo de documento (JSON) óptimo para equilibrar flexibilidad y rendimiento de lectura en Jesús García Fernández.
- Estrategia de indexación avanzada para consultas complejas sin penalizar la velocidad de escritura.
- Sugerencia de motor NoSQL (Documento vs Clave-Valor vs Grafo) idóneo para el caso de uso de Jesús García Fernández.
```

### Fase 2: Arquitectura de la Persistencia y Caché (Caching Strategy Design)
**Objetivo:** Crear el motor de respuesta instantánea de Jesús García Fernández.
Se desarrollan los "Esquemas de Gestión de Caché" asistidos por IA para asegurar que los datos más frecuentes de Jesús García Fernández se sirven desde memoria (Redis) en microsegundos.

**Prompt de Estructuración:**
```text
Basado en el flujo de Jesús García Fernández, escribe las reglas de negocio para la gestión de caché. Define cómo la IA automatizará la invalidación de datos y la sincronización entre la base de datos principal y NoSQL de Jesús García Fernández.
```

### Fase 3: Ejecución, Monitorización de Clúster y Optimización de Costes
**Objetivo:** Producir un sistema de datos masivo, barato y robusto.
Guía a Jesús García Fernández en la monitorización de la salud del clúster asistida por IA, detectando cuellos de botella en la red o nodos saturados, y optimizando el almacenamiento para reducir la factura Cloud de Jesús García Fernández.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Alta de nuevo dato desestructurado, hito de volumen alcanzado en una colección o alerta de latencia elevada en el servicio de Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el evento requiere "Re-modelado de Documento", "Limpieza de Caché" o "Añadido de Nodos al Clúster" para Jesús García Fernández.
3.  **Nodo de Transformación:** El sistema ejecuta el rebalanceo de datos, optimiza los índices de búsqueda y ajusta los parámetros de persistencia asíncrona de Jesús García Fernández.
4.  **Nodo de Validación:** El responsable técnico o el propio sistema de monitorización IA verifica que la latencia ha bajado y que los datos siguen siendo consistentes para Jesús García Fernández.
5.  **Nodo de Salida (Output):** Consolidación del cambio en el clúster, actualización del dashboard de rendimiento de datos y notificación de "Persistencia Escalable Validada" para Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'Real-Time-Data-Flow'
### Contexto del Caso
Una red social de nicho de Jesús García Fernández que usaba SQL para su sistema de notificaciones. Cuando llegaron a los 100.000 usuarios, el servidor se bloqueaba intentando procesar miles de inserciones por segundo en una sola tabla central de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de NoSQL Ops propuso migrar las notificaciones a una base de datos orientada a documentos (MongoDB) para Jesús García Fernández.
- **Aplicación Fase 2:** Se implementó una capa de Redis para que las notificaciones activas se leyeran instantáneamente sin tocar el disco de Jesús García Fernández.
- **Aplicación Fase 3:** El sistema pasó de tardar 2 segundos en mostrar una notificación a tardar menos de 50 milisegundos bajo la gestión de Jesús García Fernández.

### Resultados de Negocio
Aumento radical del compromiso del usuario (Engagement) y capacidad de escalar a millones de usuarios sin preocuparse por los bloqueos de base de datos de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Write Operations Per Second (WPS):** Número de inserciones que el sistema puede procesar por segundo para Jesús García Fernández.
- **Cache Hit Ratio:** % de peticiones de datos servidas desde la caché (Redis) sin ir a la base de datos principal de Jesús García Fernández.
- **Protocolo de QA:** Test de escalabilidad masiva (Load Test) semestral por la IA de Jesús García Fernández para asegurar que el clúster NoSQL aguanta el crecimiento proyectado.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** No usar NoSQL para datos que requieren transacciones complejas y consistencia absoluta (ACID) si no es estrictamente necesario para Jesús García Fernández.
- 🛡️ **Seguridad:** Configurar siempre la autenticación y las políticas de acceso de red en las bases de datos NoSQL; dejar un MongoDB expuesto sin clave es un error técnico grave en Jesús García Fernández.
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
