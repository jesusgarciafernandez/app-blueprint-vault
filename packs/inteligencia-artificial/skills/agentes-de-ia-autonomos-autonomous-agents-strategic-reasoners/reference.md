# Referencia ampliada — Agentes de IA Autónomos (Autonomous Agents & Strategic Reasoners)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Arquitectura de la Misión y definición de Herramientas
**Objetivo:** Definir el cerebro, las manos y los límites del agente.
1.  **Definición de 'Persona' y Meta:** IA ayuda a redactar las instrucciones de sistema que definen la personalidad táctica del agente y sus criterios de éxito claros.
2.  **Mapeo de Herramientas (Tooling):** Identificación de las funciones Python o APIs que el agente tiene permitido llamar (Ej: Acceso a Google, Ejecución de SQL).

**Prompt Maestro de Agentes Autónomos:**
```text
Actúa como un Senior Agent Architect y Experto en Sistemas Cognitivos. Diseña el agente autónomo para [MISIÓN/TAREA]. 
1. Estructura el Grafo de Decisión: Define el flujo lógico (Ej: Planificación -> Ejecución -> Revisión -> Entrega) y cómo manejaremos el 'Feedback Loop'. 
2. Definición de Herramientas Estrictas: Lista las 3 herramientas clave que el agente usará y redacta la descripción técnica de cada una para que el LLM sepa cuándo invocarlas. 
3. Lógica de 'Self-Correction': ¿Cómo evaluará el agente si un paso ha fallado y qué estrategia de 'Retry' o 'Pivot' debe seguir? 
4. Gestión de Memoria Operativa: Define qué información del paso anterior debe persistir en el contexto para que el agente no pierda el hilo en tareas largas. 
5. Protocolo de Seguridad (Kill Switch): Establece bajo qué condiciones el agente debe detenerse inmediatamente y solicitar intervención manual crítica.
```

### Fase 2: Ejecución, Monitorización y Refinamiento del Ciclo
... (Expansión técnica sobre el uso de la técnica de 'Chain-of-Thought' forzada para que el agente verbalice su plan antes de actuar, la implementación de un sistema de 'Traceability' que registre cada acción para auditoría, y la optimización de los intervalos de reflexión para balancear la rapidez de ejecución con la precisión del razonamiento) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de operación proactiva.*

1.  **Trigger:** Definición de una meta de alto nivel por parte del humano o detección de un evento complejo en el entorno.
2.  **Nodo de Planificación Cognitiva:** El agente analiza el estado actual y genera una lista de tareas (To-Do List) dinámica para alcanzar la meta.
3.  **Nodo de Acción con Herramientas:** La IA ejecuta la subtarea actual invocando la herramienta necesaria (API/Código/Búsqueda).
4.  **Nodo de Observación y Reflexión:** El sistema lee el output del paso anterior, lo compara con el objetivo y decide si continuar, corregir o escalar.
5.  **Output:** Meta alcanzada con informe de acciones realizadas; el agente entra en estado de 'Espera' hasta la siguiente misión o instrucción.

---

## 7. Ejemplo Práctico: Agencia de Growth 'AutoMarketer'
**Reto:** Necesitaban monitorizar 50 palabras clave de la competencia, identificar las 5 mejores oportunidades de contenido y redactar borradores de blog cada mañana.
**Acción v2.0:** Implementaron un Agente Autónomo (Skill 204). La IA despierta a las 08:00, busca en Google News, analiza el tráfico, decide sobre qué escribir, redacta los borradores y los deja listos para revisión en el CMS.
**Resultado:** El equipo de SEO pasó de dedicar 4 horas diarias a la investigación a solo 10 minutos de edición final. La IA incluso aprendió a detectar "neologismos del sector" de forma autónoma antes que los humanos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
