---
name: lead-scoring-inteligente-behavioral-firmographic-scoring
description: "El Lead Scoring Inteligente es el sistema de clasificación numérica de prospectos basado en su ajuste al perfil ideal y su nivel de compromiso digital. No es un sistema estático; es Ingeniería de la Prioridad Comercial. Úsala para tareas de Gestión de Leads y CRM: lead-scoring, sales-priority, crm-optimization, marketing-automation, smarketing, predictive-scoring."
title: Lead Scoring Inteligente (Behavioral & Firmographic Scoring)
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-17
category: 05. Gestión de Leads y CRM
subcategory: Cualificación y Scoring
tags: [lead-scoring, sales-priority, crm-optimization, marketing-automation, smarketing, predictive-scoring, lead-management, revenue-growth]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 129
---

## 0. Filosofía Human-Centric AI
*Esta habilidad prioriza el tiempo del equipo de ventas enfocándolos en las personas que realmente necesitan y están listas para su ayuda, utilizando la tecnología para detectar la intención de compra sin ser intrusivo.*

**El Rol del Humano:** El Especialista en Cualificación debe ser un "Arquitecto del Criterio". La IA puede rastrear clics, visitas a la página de precios y descargas de documentos para asignar puntos de forma instantánea, pero solo el humano puede evaluar si un pico de actividad es un interés real o solo curiosidad académica, decidir qué hitos de comportamiento son verdaderamente "críticos" para la venta y asegurar que la automatización no deshumanice la relación inicial con el prospecto.
**Empoderamiento:** Usamos la tecnología para separar el "grano de la paja" automáticamente, permitiendo que el equipo comercial se despierte cada día con una lista priorizada de contactos "Hot" que están esperando su llamada.

---

## 1. Descripción Detallada
El Lead Scoring Inteligente es el sistema de clasificación numérica de prospectos basado en su ajuste al perfil ideal y su nivel de compromiso digital. No es un sistema estático; es **Ingeniería de la Prioridad Comercial**. El enfoque v2.0 incorpora el **Scoring Predictivo y Negativo**, donde el sistema no solo suma puntos por acciones positivas, sino que los resta por comportamientos que indican falta de intención (como visitar la sección de empleo) o desajuste con el perfil (Negative Persona), garantizando que solo los MQLs (Marketing Qualified Leads) de mayor calidad lleguen al equipo de ventas.

## 2. Escenarios de Aplicación
- **Gestión de Grandes Volúmenes de Leads:** Priorización automática cuando el equipo de ventas está desbordado por el marketing masivo.
- **Identificación de 'Sales Ready Leads':** Alerta inmediata cuando un lead atraviesa el umbral de puntuación que indica madurez de compra.
- **Optimización de Campañas de Nurturing:** Personalización del contenido enviado según el nivel de interés detectado.
- **Limpieza de Bases de Datos:** Identificación de contactos "zombis" o irrelevantes para su eliminación o re-captura estratégica.
- **Alineación Smarketing (Marketing + Ventas):** Establecimiento de reglas comunes para definir qué es un "buen lead", reduciendo conflictos internos.

## 3. Requisitos de Implementación
- **CRM con Motor de Reglas Dinámicas:** Hubspot, Salesforce o similar con capacidad de cálculo de propiedades en tiempo real.
- **Tracking de Comportamiento Digital:** Integración de la web con el CRM para capturar visitas a páginas específicas, descargas y clics.
- **Definición de Matriz de Scoring:** Documento consensuado que asigne valores a datos (Cargo, Industria, Tamaño) y comportamientos (Email opens, Web visits).
- **Historial de Ventas para Validación:** Datos previos para asegurar que los puntos asignados correlacionan realmente con la probabilidad de cierre.

---

## 4. Diferencial: Scoring Básico vs. Scoring Inteligente v2.0

| Dimensión | Scoring Genérico (Legacy) | Scoring Inteligente (v2.0) |
| :--- | :--- | :--- |
| **Lógica** | Solo suma puntos. | Suma, resta y multiplica (Scoring Negativo). |
| **Tiempo** | Los puntos son eternos. | Degradación de puntos por inactividad (Time Decay). |
| **Fuente de Datos** | Solo datos del formulario. | Datos de uso de producto, emails y web. |
| **Actualización** | Manual y periódica. | En tiempo real por cada interacción. |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Diseño de la Matriz de Puntuación (Explicit & Implicit)
**Objetivo:** Crear el algoritmo de puntuación que refleje la realidad del negocio.
1.  **Scoring Explícito (Perfil):** Asigna puntos por coincidencia con el ICP (Ej: Director de IT = +20 pts, Estudiante = -100 pts).
2.  **Scoring Implícito (Acción):** Asigna puntos por "señales de vida" (Ej: Visita página de precios = +15 pts, Clic en email = +5 pts).

**Prompt Maestro de Configuración de Lead Scoring:**
```text
Actúa como un Experto en Marketing Automation y CRM Analytics. Diseña el modelo de Lead Scoring para [MODELO_NEGOCIO/EMPRESA]. 
1. Define los 5 campos demográficos críticos y sus puntuaciones: [Cargo, Tamaño Empresa, Ubicación, etc.]. 
2. Establece la lógica de 'Puntuación por Comportamiento': ¿Cuántos puntos damos por una demo, por ver 3 posts del blog o por un abandono de carrito? 
3. Implementa el 'Time Decay': ¿Cuánta puntuación pierde un lead tras 2 semanas de inactividad total? 
4. Define el umbral de 'Sales Ready': ¿A cuántos puntos notificamos al equipo de ventas? 
5. Crea 3 reglas de 'Scoring Negativo' para filtrar contactos no deseados.
```

### Fase 2: Automatización, Alertas y Ciclo de Feedback
... (Expansión técnica sobre la creación de workflows de alerta en Slack, la reasignación automática de leads "Hot" y la revisión trimestral de la efectividad del modelo) ...

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
