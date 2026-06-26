---
name: diseno-estrategico-orientado-al-dominio-domain-driven-design-ddd
description: "El Diseño Estratégico Orientado al Dominio o DDD (v2.0) es la metodología definitiva para gestionar la complejidad en proyectos de software de gran escala. No es solo \"organizar carpetas\"; es Ingeniería del Modelo de Negocio Sintético. Úsala para tareas de Desarrollo de Software: ddd, arquitectura, dominio, lenguaje-ubicuo, modelado, estrategia."
title: Diseño Estratégico Orientado al Dominio (Domain-Driven Design / DDD)
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-18
category: 16. Desarrollo de Software
subcategory: 16.4 Arquitectura de Software
tags: [ddd, arquitectura, dominio, lenguaje-ubicuo, modelado, estrategia, bounded-context, event-storming, ubiquitous-language, aggregates, value-objects, strategic-design]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 237
---

## 0. Filosofía Human-Centric AI
*Esta habilidad alinea el lenguaje de las personas con el lenguaje de las máquinas, utilizando el Diseño Orientado al Dominio (DDD) para que el software sea un reflejo fiel de la realidad del negocio y permitir que el humano hable y construya tecnología en sus propios términos, reduciendo la brecha entre la ambición estratégica y la ejecución técnica.*

**El Rol del Humano:** El Arquitecto del Lenguaje Ubicuo debe ser un "Garantes del Sentido y la Coherencia". La IA puede sugerir estructuras de objetos, identificar fronteras lógicas preliminares y generar plantillas de código basadas en modelos de dominio, pero solo el humano posee la capacidad de extraer los matices sutiles de la operativa real a través del diálogo con expertos, decidir los límites de los contextos acotados que definen la organización y asegurar que la tecnología no sea un fin en sí misma, sino un vehículo transparente para resolver los problemas del negocio.
**Empoderamiento:** Usamos la tecnología para sustituir la confusión técnica por una arquitectura basada en el lenguaje y la realidad humana.

---

## 1. Descripción Detallada
El Diseño Estratégico Orientado al Dominio o **DDD** (v2.0) es la metodología definitiva para gestionar la complejidad en proyectos de software de gran escala. No es solo "organizar carpetas"; es **Ingeniería del Modelo de Negocio Sintético**. El enfoque v2.0 se centra en el **Lenguaje Ubicuo y los Contextos Acotados (Bounded Contexts)**: la creación de un idioma común entre expertos de negocio y desarrolladores que se refleja directamente en el código. Abarca el uso de patrones estratégicos (Context Mapping) para definir cómo se comunican las diferentes áreas de la empresa y patrones tácticos (Aggregates, Entities, Value Objects) para asegurar la integridad de la lógica de negocio en cada módulo independiente.

## 2. Escenarios de Aplicación
- **Modelado de Sistemas Transaccionales Complejos:** Diseño de plataformas de banca o logística donde un término como "Pedido" puede tener significados diferentes para Ventas, Almacén y Contabilidad.
- **Transición a Arquitecturas de Microservicios:** Uso de DDD para encontrar las "costuras" naturales del sistema y dividir el monolito en servicios independientes basados en funciones de negocio reales.
- **Proyectos de Larga Duración y Alta Rotación:** Creación de un código base que se explica a sí mismo a través de su lenguaje, facilitando que nuevos ingenieros entiendan el negocio leyendo el código.
- **Refactorización de 'Big Ball of Mud':** Técnica para limpiar sistemas donde la lógica está mezclada, aislando el núcleo de negocio (Domain Core) de los detalles de infraestructura.
- **Sesiones de Event Storming:** Facilitación de talleres visuales donde negocio e IT mapean el flujo de eventos de la empresa para descubrir el modelo de dominio oculto.

## 3. Requisitos de Implementación
- **Dominio de Patrones Estratégicos:** Capacidad para diseñar el 'Context Map' de una organización y establecer relaciones (Upstream/Downstream).
- **Habilidad en Patrones Tácticos:** Implementación técnica de Aggregates profundos, Repositories, Domain Services y Value Objects inmutables.
- **Facilitación de Talleres de Modelado:** Uso de técnicas de 'Event Storming' o 'Domain Storytelling' para extraer conocimiento de los expertos.
- **Comunicación Transversal:** Habilidad para negociar términos y definiciones con directivos, operativos y desarrolladores simultáneamente.

---

## 4. Diferencial: Arquitectura por Capas vs. Domain-Driven Design v2.0

| Dimensión | Enfoque Legacy (Data-Driven) | DDD Estratégico (v2.0) |
| :--- | :--- | :--- |
| **Inicio** | Empieza por la Base de Datos. | Empieza por el Modelo de Negocio. |
| **Lenguaje** | Términos técnicos (DAO, Controller). | Términos de negocio (Invoice, Route). |
| **Fronteras** | Definidas por la tecnología. | Definidas por contextos de negocio. |
| **Complejidad** | Se acumula en funciones gigantes. | Se distribuye en objetos con significado. |

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
