# Referencia ampliada — Planificación Táctica y Bloqueo de Tiempo (Weekly & Daily Flow Design)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Capacidad y Diseño del 'Calendario Maestro'
**Objetivo:** Establecer las reglas de juego y los bloques inamovibles.
1.  **Definición de 'Rocas del Sistema':** IA ayuda a identificar las 3-5 tareas estratégicas de la semana que no pueden fallar.
2.  **Arquitectura del Time Blocking Semanal:** Reserva de bloques para Deep Work, Comunicación, Administración y Descanso en el calendario.

**Prompt Maestro de Planificación Táctica (Flow Architect):**
```text
Actúa como un Senior Productivity Consultant y Diseñador de Workflows de Alto Rendimiento. Diseña el plan de ejecución semanal para: [USUARIO/PROYECTO]. 
1. Estructura de Bloques Semanales: Propón una distribución de bloques para [DESCRIBIR_PERFIL] (Ej: Mañanas rojas para Deep Work, Tardes azules para reuniones). 
2. Algoritmo de Estimación de Tiempo: Define una regla (Ej: Tiempo estimado x 1.5) para aplicar a todas las tareas basándote en la Ley de Hofstadter. 
3. Ritual de Planificación Diaria (Shutdown): Redacta los 5 minutos de pasos que debo seguir al final del día para dejar organizada la mañana siguiente. 
4. Diseño de 'Buffers' de Emergencia: ¿Cómo y cuándo reservaremos tiempo para los imprevistos que surjen cada día sin que rompan la planificación? 
5. Protocolo de Revisión Domingos/Lunes: Diseña el checklist para la organización de la semana entrante, alineándola con los objetivos del mes.
```

### Fase 2: Ejecución, Navegación de la Agenda y Ajuste Dinámico
... (Expansión técnica sobre el uso de la técnica de 'Calendar Auditing' para detectar fugas de tiempo, la implementación de un proceso de 'Priorización Diaria 1-3-5', y la monitorización de la 'Métrica de Adherencia al Plan' para aprender de las desviaciones y mejorar la precisión futura) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de tiempo soberano.*

1.  **Trigger:** Final de semana, final de día o adición de una tarea con fecha crítica al sistema.
2.  **Nodo de Sugerencia de Bloque:** El sistema analiza las horas libres en el calendario y el tipo de tarea, sugiriendo el mejor momento para su ejecución (Ej: Tarea creativa en la franja de máxima energía).
3.  **Nodo de Sincronización Automática:** El sistema bloquea el tiempo en el calendario al marcar una tarea como 'Prioridad 1' en el gestor de tareas.
4.  **Nodo de Alerta de Saturación:** El sistema lanza un aviso visual si el usuario intenta planificar más del 70% de sus horas laborales, forzando la reserva de buffers.
5.  **Output:** Calendario realista y alineado; reducción de la ansiedad por lo pendiente; mayor índice de tareas completadas a tiempo; equilibrio vital preservado.

---

## 7. Ejemplo Práctico: El Freelance 'Desbordado'
**Reto:** Ana, diseñadora freelance, nunca sabía si podía aceptar un nuevo encargo. Sus listas de tareas eran kilométricas pero al final del día sentía que solo había hecho correos basura. Trabajaba fines de semana para compensar.
**Acción v2.0:** Implementó Skill 270. Empezó a usar Google Calendar para TODO. Bloqueó sus mañanas para "Diseño Puro" (sin internet) y dejó las tardes para "Gestión y Cliente". Reservó 1 hora de buffer después de comer para las urgencias que siempre le enviaban por la mañana.
**Resultado:** Ana ahora sabe exactamente cuándo puede entregar un proyecto (mira su calendario, no su lista). Ha dejado de trabajar los fines de semana porque su capacidad real es ahora visible. Su calidad de diseño ha subido al poder dedicar bloques de 4 horas ininterrumpidas a cada cliente.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
