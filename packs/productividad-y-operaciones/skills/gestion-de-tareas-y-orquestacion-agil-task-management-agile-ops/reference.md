# Referencia ampliada — Gestión de Tareas y Orquestación Ágil (Task Management & Agile Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Carga y Diseño del Ecosistema de Gestión
**Objetivo:** Elegir la herramienta adecuada y configurar el flujo de vida de la tarea.
1.  **Selección del 'Tech Stack' de Gestión:** IA ayuda a decidir si el proyecto requiere la agilidad de Todoist, la estructura de Linear o la potencia corporativa de Jira.
2.  **Diseño del Flujo de Estados (Workflow Architect):** Definición de las etapas por las que pasa una tarea (Ej: Backlog -> Discovery -> Doing -> Review -> Done).

**Prompt Maestro de Orquestación de Tareas (Task Architect):**
```text
Actúa como un Senior Project Manager y Experto en Metodologías Ágiles. Diseña el sistema de gestión para: [PROYECTO/EQUIPO]. 
1. Configuración de la Herramienta [TODOIST/JIRA/LINEAR]: Define las etiquetas maestras, filtros de prioridad y la estructura de proyectos/carpetas. 
2. Diseño del Workflow Personalizado: Propón los estados de ticket y las transiciones automáticas necesarias para eliminar el trabajo manual de actualización. 
3. Definición de Atributos de Tarea: ¿Qué información mínima debe tener cada ticket para ser ejecutable (Ej: Story Points, Due Date, Labels, Description)? 
4. Implementación de Automatizaciones Core: Describe 3 reglas (Ej: "Si un ticket se marca como 'Bug' con prioridad alta, notificar a Slack e insertar en el Sprint actual"). 
5. Protocolo de 'Backlog Grooming': Diseña la rutina semanal para limpiar tareas obsoletas y asegurar que la prioridad superior es siempre la real.
```

### Fase 2: Ejecución, Seguimiento de Velocidad y Mejora Continua
... (Expansión técnica sobre el uso de la técnica de 'Time Boxing' integrada en el gestor, la implementación de un proceso de 'Póker de Planificación' automatizado, y la monitorización de las 'Métricas de Velocidad' y 'Cycle Time' para optimizar la capacidad de entrega del equipo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de progreso imparable.*

1.  **Trigger:** Entrada de una idea, requerimiento de cliente o detección automática de un fallo en el sistema.
2.  **Nodo de Clasificación y Asignación Inteligente:** El sistema analiza la entrada, crea la tarea en la herramienta adecuada y asigna responsable y prioridad inicial.
3.  **Nodo de Enriquecimiento de Contexto:** La IA añade a la tarea documentos relacionados, transcripciones previas e hilos de Slack para que quien la ejecute tenga todo a mano.
4.  **Nodo de Monitorización y Alerta de Bloqueos:** El sistema detecta si una tarea lleva demasiado tiempo en un estado o si falta información, lanzando una alerta al responsable.
5.  **Output:** Backlog ordenado; equipo con carga de trabajo equilibrada; visibilidad total del progreso; entregables completados en tiempo y forma.

---

## 7. Ejemplo Práctico: Agencia de Desarrollo 'DevStack'
**Reto:** En 'DevStack' usaban un grupo de WhatsApp y un Excel para gestionar los proyectos. Los desarrolladores no sabían qué era urgente, los clientes preguntaban a cada hora por el estado de sus pedidos y se perdían correos con cambios críticos.
**Action v2.0:** Implementaron Skill 266. Migraron todo a Linear integrado con Slack. Crearon automatizaciones que crean tickets desde los correos de clientes y notifican al canal de proyecto cuando un hito se completa.
**Resultado:** Las reuniones de estatus bajaron de 5 semanales a 1 quincenal. La transparencia es total para los clientes mediante un dashboard de solo lectura. El equipo de desarrollo tiene un 30% menos de estrés al tener su lista de prioridades clara y centralizada.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
