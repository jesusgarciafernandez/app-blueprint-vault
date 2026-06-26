---
name: documentacion-estrategica-de-decisiones-de-arquitectura-adr-mast
description: "La Documentación de Decisiones de Arquitectura (ADR) es la práctica de capturar formalmente las elecciones técnicas críticas, su contexto, las alternativas consideradas y las consecuencias resultantes. No es solo \"escribir documentación\"; es Ingeniería de la Memoria Técnica. Úsala para tareas de Estrategia y Operaciones: adr, architectural-decision-records, tech-governance, engineering-culture, knowledge-management, architecture-design."
title: Documentación Estratégica de Decisiones de Arquitectura (ADR Mastery)
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-17
category: 08. Estrategia y Operaciones
subcategory: 08.4 Procesos y Metodologías
tags: [adr, architectural-decision-records, tech-governance, engineering-culture, knowledge-management, architecture-design, technical-debt, decision-logs, software-engineering]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 144
---

## 0. Filosofía Human-Centric AI
*Esta habilidad preserva la sabiduría colectiva y el razonamiento humano tras cada elección crítica, utilizando la tecnología para evitar la amnesia técnica y asegurar que la evolución del sistema sea coherente, ética y fundamentada.*

**El Rol del Humano:** El Arquitecto de Decisiones debe ser un "Historiador del Futuro". La IA puede resumir debates técnicos, comparar especificaciones de diferentes herramientas y generar borradores de ADR basados en actas de reuniones, pero solo el humano puede evaluar el impacto a largo plazo de una decisión en la moral del equipo, entender las sutiles presiones de negocio que fuerzan un 'Trade-off' específico y asegurar que la arquitectura respete los valores de simplicidad, sostenibilidad y responsabilidad que definen la cultura de ingeniería de la empresa.
**Empoderamiento:** Usamos la tecnología para sistematizar la captura del "Por qué" (y no solo del "Qué"), permitiendo que el conocimiento fluya sin fricciones entre las generaciones actuales y futuras de desarrolladores.

---

## 1. Descripción Detallada
La Documentación de Decisiones de Arquitectura (ADR) es la práctica de capturar formalmente las elecciones técnicas críticas, su contexto, las alternativas consideradas y las consecuencias resultantes. No es solo "escribir documentación"; es **Ingeniería de la Memoria Técnica**. El enfoque v2.0 incorpora la **Gobernanza Ágil de Arquitectura**, donde el ADR no es un trámite burocrático, sino una herramienta viva que facilita el consenso, reduce la deuda técnica acumulada por falta de contexto y permite que el equipo escale sin perder la visión original del sistema (Architecture Guardrails).

## 2. Escenarios de Aplicación
- **Elección de Frameworks o Lenguajes:** Justificación de por qué se prefirió Next.js sobre Remix, o Python sobre Go en un módulo específico.
- **Definición de Patrones de Comunicación:** Registro del acuerdo de usar gRPC en lugar de REST para microservicios internos.
- **Cambios en la Estrategia de Base de Datos:** Documentación del paso de una DB Relacional a una Grafo basándose en requerimientos de escalabilidad.
- **Onboarding Acelerado de Ingeniería:** Facilita que los nuevos miembros lean la "historia de decisiones" para entender el estado actual del código.
- **Auditoría de Deuda Técnica:** Identificación de decisiones pasadas que ya no son válidas por cambios en el mercado o la tecnología.

## 3. Requisitos de Implementación
- **Repositorio Centralizado de ADRs:** Carpeta `/docs/adr` en el mismo repositorio de código para máxima visibilidad (Markdown format).
- **Consenso de Equipo:** Proceso claro de revisión y aprobación de ADRs (Pull Requests).
- **Template Estándar de Alta Densidad:** Uso de formatos probados (Nygard, MADR) que obliguen a pensar en el contexto y las consecuencias.

---

## 4. Diferencial: Documentación Estática vs. ADR Mastery v2.0

| Dimensión | Documentación Clásica (Legacy) | ADR Mastery (v2.0) |
| :--- | :--- | :--- |
| **Ubicación** | Wiki externa / PDF olvidado. | En el código (Git), junto a la implementación. |
| **Enfoque** | ¿Cómo funciona esto ahora? | ¿Por qué decidimos que funcionara así? |
| **Impacto** | Descriptivo y estático. | Normativo y evolutivo. |
| **Visibilidad** | Nadie la lee tras 3 meses. | Es parte obligatoria del flujo de desarrollo. |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Identificación y Registro del Contexto
**Objetivo:** Capturar la "foto del momento" antes de que se olvide el razonamiento.
1.  **Detección de 'Architectural Significance':** ¿Esta decisión afectará a más de un equipo? ¿Es difícil de revertir? Si es así, requiere un ADR.
2.  **Mapeo de Alternativas (Trade-offs):** Lista las otras 2 opciones descartadas y por qué perdieron frente a la elegida.

**Prompt Maestro de Generación de ADR:**
```text
Actúa como un Principal Software Architect. Redacta un ADR (Architectural Decision Record) Profesional para [PROBLEMA/DECISIÓN]. 
1. Título y Estatus: [Propuesto, Aceptado, Superado]. 
2. Contexto: ¿Qué problema de negocio o técnico estamos resolviendo? [Ej: Latencia, Coste, Escalabilidad]. 
3. Decisión: ¿Qué vamos a hacer exactamente? 
4. Consecuencias: Sé honesto, indica lo positivo (Beneficios) y lo negativo (Trade-offs/Deuda técnica). 
5. Alternativas: ¿Qué otras 2 opciones evaluamos y por qué no las elegimos?
6. Formato: Markdown estructurado compatible con el estándar Michael Nygard.
```

### Fase 2: Socialización, Aprobación y Evolución
... (Expansión técnica sobre el proceso de revisión de ADRs vía PR, la vinculación de ADRs con tareas de Jira/Linear y el reporte de 'Entropía de Decisiones' para detectar cuándo una arquitectura está quedando obsoleta) ...

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
