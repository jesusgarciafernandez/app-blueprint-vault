# Referencia ampliada — Agrupación Estratégica de Lotes (Task Batching & Flow Alignment)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Fragmentación y Diseño de 'Lotes Maestros'
**Objetivo:** Identificar las tipologías de tareas y asignarles su espacio vital.
1.  **Inventario de Tipos de Tarea:** IA ayuda a analizar el backlog de la semana pasada para identificar cuáles se repiten y cuáles comparten el mismo "entorno mental".
2.  **Diseño de la Arquitectura de la Agenda:** Creación de bloques recurrentes en el calendario para cada gran tipología de lote detectada.

**Prompt Maestro de Arquitectura de Lotes (Batch Architect):**
```text
Actúa como un Senior Operations Manager y Experto en Productividad de Alto Rendimiento. Diseña el sistema de batching para: [PERFIL/PROYECTO]. 
1. Definición de Lotes por Contexto: Propón 4 grandes categorías de lotes basándote en un flujo de trabajo de [DESCRIBIR_ACTIVIDAD_PRINCIPAL]. 
2. Planificación de Bloques en Calendario: Diseña una 'Semana Tipo' donde los bloques de comunicación no interrumpan las fases de trabajo profundo. 
3. Reglas de Filtrado de Lotes: Define qué criterios debe cumplir una tarea para entrar en el lote de 'Administración' vs 'Estratégico'. 
4. Automatización de la Clasificación: Describe cómo usaremos etiquetas en [TODOIST/JIRA/ASANA] para que al abrir el gestor, las tareas ya aparezcan agrupadas por lote. 
5. Protocolo de Gestión de Emergencias: ¿Cómo manejaremos una interrupción real sin romper el modo de batching? (Ej: La técnica del 'Interruption Log').
```

### Fase 2: Ejecución, Refinamiento de Ritmos y Auditoría de Flujo
... (Expansión técnica sobre el uso de la técnica de 'Theme Days' para simplificar el batching a escala semanal, la implementación de un proceso de 'Batch Processing' para tareas administrativas repetitivas, y la monitorización de la 'Métrica de Cambio de Contexto' para asegurar la salud mental del equipo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de ritmo inalterable.*

1.  **Trigger:** Adición de una nueva tarea al sistema o inicio de un nuevo periodo de planificación.
2.  **Nodo de Etiquetado y Categorización Automática:** El sistema analiza la descripción de la tarea y le asigna el 'Tag de Contexto' adecuado basándose en el aprendizaje previo.
3.  **Nodo de Sugerencia de Bloque:** El sistema muestra la tarea solo cuando el usuario entra en el bloque de tiempo correspondiente en su calendario.
4.  **Nodo de Blindaje de Atención:** Durante la ejecución del lote, el sistema silencia automáticamente todos los canales de entrada que no pertenezcan a ese lote.
5.  **Output:** Agenda equilibrada; mayor velocidad de entrega (Lead Time); reducción del agotamiento por multitarea; equipo en estado de flujo sincronizado.

---

## 7. Ejemplo Práctico: Agencia 'ContentFlow'
**Reto:** En 'ContentFlow' los redactores pasaban el día respondiendo a clientes por Slack mientras intentaban escribir artículos. Tardaban 4 horas en un post de 500 palabras porque los interrumpían cada 10 minutos.
**Acción v2.0:** Implementaron Skill 264. Definieron "Mañanas de Creación" (08:00 a 12:00) con Slack cerrado. Todas las dudas de clientes se resuelven en un lote único de 12:00 a 13:00 y otro al final del día.
**Resultado:** La velocidad de redacción se triplicó. Los redactores terminan su trabajo con más energía y la calidad de los textos subió al poder dedicarles atención ininterrumpida. Los clientes están igual de contentos porque saben exactamente cuándo recibirán respuesta.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
