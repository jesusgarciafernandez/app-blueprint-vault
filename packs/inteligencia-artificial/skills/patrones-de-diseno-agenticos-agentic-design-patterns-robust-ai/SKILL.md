---
name: patrones-de-diseno-agenticos-agentic-design-patterns-robust-ai
description: "Patrones de Diseño Agénticos (v2.0) es la competencia de aplicar estructuras arquitectónicas recurrentes para mejorar el rendimiento de los LLMs en tareas autónomas. No es solo \"pedirle a la IA que haga cosas\"; es Arquitectura del Razonamiento Sintético. Úsala para tareas de Inteligencia Artificial: ia, agentes, design-patterns, reflection, planning, tool-use."
title: Patrones de Diseño Agénticos (Agentic Design Patterns & Robust AI)
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-18
category: 15. Inteligencia Artificial
subcategory: 15.2 Automatización Agéntica
tags: [ia, agentes, design-patterns, reflection, planning, tool-use, multi-agent, agentic-workflows, robustness, prompt-engineering-v2, autonomous-logic]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 202
---

## 0. Filosofía Human-Centric AI
*Esta habilidad establece las leyes fundamentales de construcción para sistemas de inteligencia artificial autónomos, utilizando la tecnología para implementar estructuras de razonamiento probadas (patrones) y permitir que el humano diseñe agentes que no solo responden, sino que piensan, planifican y aprenden de sus propios errores de manera robusta y predecible.*

**El Rol del Humano:** El Arquitecto de Patrones Agénticos debe ser un "Garantes de la Maestría Estructural". La IA puede seguir instrucciones complejas y ejecutar ciclos de mejora continua (Reflexión), pero solo el humano puede definir la arquitectura que garantiza la estabilidad del sistema, elegir el patrón adecuado para cada desafío de negocio (Ej: ¿Necesitamos un agente que planifique o uno que reaccione?) y asegurar que los bucles de autonomía de la IA incluyan puntos de control humano que eviten la deriva algorítmica o la ejecución de acciones indeseadas.
**Empoderamiento:** Usamos la tecnología para sustituir la improvisación en el prompting por una ingeniería de software aplicada a la inteligencia artificial.

---

## 1. Descripción Detallada
Patrones de Diseño Agénticos (v2.0) es la competencia de aplicar estructuras arquitectónicas recurrentes para mejorar el rendimiento de los LLMs en tareas autónomas. No es solo "pedirle a la IA que haga cosas"; es **Arquitectura del Razonamiento Sintético**. El enfoque v2.0 se basa en los 4 pilares de Andrew Ng: **Reflexión** (el agente revisa su propio trabajo), **Planificación** (desglose de metas en pasos), **Uso de Herramientas** (interacción con APIs/DBs) y **Colaboración Multi-Agente** (división de roles). El objetivo es pasar de una interacción de "un solo disparo" (Zero-shot) a flujos de trabajo iterativos (Agentic Workflows) que multiplican la precisión y fiabilidad del sistema.

## 2. Escenarios de Aplicación
- **Sistemas de Self-Correction para Código:** Agentes que escriben código, lo intentan ejecutar, leen el error en la consola y se auto-corrigen hasta que el test unitario pasa (Patrón de Reflexión).
- **Planificación de Proyectos de Marketing:** Un agente que primero diseña un cronograma detallado de 10 pasos y luego ejecuta cada paso secuencialmente, ajustando el plan si surge un imprevisto (Patrón de Planificación).
- **Asistentes de Investigación con Herramientas Reales:** Agentes que saben cuándo buscar en Google, cuándo leer un PDF local y cuándo consultar una base de datos SQL para responder (Patrón de Tool-use).
- **Flujos de Debate para Calidad Extrema:** Uso de dos agentes con visiones contrapuestas (Crítico vs Creador) para refinar un documento hasta alcanzar la excelencia (Patrón Multi-Agente).
- **Pipelines de Extracción de Datos Resistentes a Errores:** Sistemas que validan el formato de salida y, si no es el correcto, reintento la tarea con un prompt de corrección automático.

## 3. Requisitos de Implementación
- **Entendimiento de Cadenas de Pensamiento (CoT):** Conocimiento de cómo guiar al modelo para que "piense en voz alta" antes de actuar.
- **Frameworks de Orquestación Agéntica:** Uso de LangChain, CrewAI, AutoGen o PydanticAI para implementar la jerarquía de llamadas.
- **Domino de Esquemas Estructurados (JSON/Pydantic):** Capacidad para forzar salidas que los sistemas de software puedan procesar de forma determinista.
- **Gestión de 'State' y Memoria:** Habilidad para pasar el estado de la tarea entre diferentes iteraciones del agente sin pérdida de información.

---

## 4. Diferencial: Prompting Lineal vs. Patrones Agénticos v2.0

| Dimensión | Enfoque Legacy (Zero-shot) | Patrones Agénticos (v2.0) |
| :--- | :--- | :--- |
| **Precisión** | Baja; acierto a la primera o fallo. | Muy alta; el sistema itera hasta acertar. |
| **Complejidad** | Limitada a tareas simples. | Capaz de resolver misiones multi-etapa. |
| **Fiabilidad** | Impredecible; depende del "humor" del modelo. | Determinista; basada en protocolos de validación. |
| **Autonomía** | Requiere que el humano guíe cada paso. | El humano define la meta y el patrón guía la ejecución. |

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
