---
name: interaction-design-ixd-diseno-de-comportamiento-y-feedback-siste
description: "El Diseño de Interacción (IxD) es la disciplina que define el comportamiento de los productos digitales en respuesta a las acciones del usuario. No es solo \"hacer que se mueva\": es Ingeniería del Diálogo Dinámico. Úsala para tareas de Generación de Contenido: interaction-design, ixd, micro-interactions, affordance, feedback-loops, cognitive-load."
title: Interaction Design (IxD), Diseño de Comportamiento y Feedback Sistémico
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-17
category: 02. Generación de Contenido
subcategory: Diseño UI
tags: [interaction-design, ixd, micro-interactions, affordance, feedback-loops, cognitive-load, protopie, framer, ia-interaction-logic]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 072
---

## 0. Filosofía Human-Centric AI
*Esta habilidad dota de alma y reactividad a la materia digital, utilizando la tecnología para crear un diálogo fluido y natural que respeta el ritmo del pensamiento humano.*

**El Rol del Humano:** El Diseñador de Interacción debe ser un "Coreógrafo del Diálogo Hombre-Máquina". La IA puede predecir qué botón se pulsará a continuación y automatizar las transiciones visuales, pero solo el humano puede imbuir al sistema de una "personalidad" reactiva coherente, decidir cuándo un feedback es intrusivo o tranquilizador, y asegurar que cada interacción potencie la sensación de control y maestría del usuario, evitando la frustración y la confusión cognitiva.
**Empoderamiento:** Usamos la tecnología para automatizar la lógica de estados complejos y simular flujos de interacción masivos, permitiendo que el experto se centre en la elegancia del diálogo y en la excelencia de la ergonomía digital.

---

## 1. Descripción Detallada
El Diseño de Interacción (IxD) es la disciplina que define el comportamiento de los productos digitales en respuesta a las acciones del usuario. No es solo "hacer que se mueva": es **Ingeniería del Diálogo Dinámico**. El enfoque v2.0 incorpora la **Interacción Predictiva y el Feedback Multisensorial**, donde se orquestan los 5 principios base (Visibilidad, Affordance, Mapeo, Feedback y Restricciones) para crear interfaces que operen con una fluidez casi biológica, minimizando la carga cognitiva y maximizando la eficiencia operativa en cualquier contexto de entrada (Touch, Mouse, Voz o Gesto).

## 2. Escenarios de Aplicación
- **Definición de Comportamientos en Design Systems:** Creación de las reglas de cómo responde cada componente ante el 'hover', 'clic', 'error' o 'carga'.
- **Interacción en Dispositivos Móviles y Wearables:** Diseño de gestos naturales (Swipes, Force-touch) que se sientan intuitivos y físicos.
- **Interfaces para Contextos de Alta Tensión (Sanidad/Emergencias):** Interacciones breves, claras y con feedback contundente que no dejen lugar a la duda.
- **Dashboards de Control de Datos Complejos:** Diseño de la interacción de filtrado, zoom y desglose que no pierda el contexto del usuario.
- **Humanización de Bots y Sistemas Autónomos:** Creación de micro-interacciones que indican que el sistema está "pensando" o "atendiendo".

## 3. Requisitos de Implementación
- **Maestría en las 5 Dimensiones de Interaction Design:** Palabras, Representaciones visuales, Objetos físicos/espacio, Tiempo y Comportamiento.
- **Dominio de Leyes de Psicología Aplicadas:** Ley de Fitts (destreza motora), Ley de Hick (toma de decisiones) y el Efecto de Posición Serial.
- **Uso de Herramientas de Prototipado Lógico:** Protopie, Framer o el motor avanzado de Smart Animate en Figma para validar comportamientos complejos antes de programar.

---

## 4. Diferencial: Pantallas Estáticas vs. Interacción Dinámica v2.0

| Dimensión | Enfoque "Páginas con enlaces" | Diseño de Interacción (v2.0) |
| :--- | :--- | :--- |
| **Respuesta** | Discontinua / Saltos bruscos. | Fluida / Estados de transición suaves. |
| **Claridad** | El usuario "prueba a ver qué pasa". | Affordance claro (Sé para qué sirve antes de tocar). |
| **Feedback** | Solo tras completar la acción. | Feedback inmediato y progresivo durante la acción. |
| **Control** | El sistema dicta el ritmo. | El sistema se adapta al modelo mental del usuario. |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Affordance y Diseño del Mapa de Estados
**Objetivo:** Asegurar que cada elemento "pida" ser usado correctamente y el sistema responda.
1.  **Auditoría de Affordance:** ¿Parece un botón? ¿Parece que se puede arrastrar? Ajusta sombras y relieves para que la función sea obvia sin palabras.
2.  **Mapeo de Estados de Componente:** Define para cada pieza: [Inactivo / Hover / Pulsado / Cargando / Éxito / Error].

**Prompt Maestro de Dirección de Interaction Design:**
```text
Actúa como Diseñador de Interacción (IxD) Senior y Especialista en Prototipado Lógico. Para la interacción [ACCIÓN_USUARIO], realiza el siguiente plan de comportamiento: 
1. Define la 'Gramática de Gestos': ¿Qué acciones físicas (Tap, Double tap, Long press) activan qué funciones? 
2. Diseña el 'Bucle de Feedback': Qué señales visuales y hápticas (vibración) recibe el usuario en tiempo real mientras realiza la acción. 
3. Establece el 'Timing y Easing' de las transiciones: [Ej: Inercia suave hacia el final para que se sienta natural]. 
4. Documenta las 'Restricciones de Uso': Cómo evitamos que el usuario cometa un error irreversible (Ej: Diálogos de confirmación destructiva). 
5. Protocolo de 'Multimodalidad': Cómo se comporta esta interacción si el usuario cambia el dedo por un Apple Pencil o el teclado.
```

### Fase 2: Prototipado Funcional, Validación de 'Maestría' y Handoff Lógico
... (Expansión técnica sobre el diseño de la 'Continuidad Visual' entre pantallas, la calibración de la latencia percibida y la entrega de especificaciones de animación -curvas Bezier y duraciones- al equipo de desarrollo) ...

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
