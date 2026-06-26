# Referencia ampliada — Delegación Inteligente y Gestión de la Capacidad (Strategic Delegation)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Tiempo y Diseño del Paquete de Delegación
**Objetivo:** Identificar qué delegar y cómo transmitir el conocimiento.
1.  **Análisis de Valor de Tarea:** IA ayuda a clasificar las tareas del usuario por 'Gozabilidad' vs 'Impacto de Negocio', identificando los candidatos ideales para delegar (Bajo valor/Baja gozabilidad).
2.  **Creación del 'Kit de Inicio' (SOP):** Grabación de un proceso real realizando la tarea y su transcripción estructurada en pasos.

**Prompt Maestro de Diseño de Delegación (Capacity Architect):**
```text
Actúa como un Senior Operations Manager y Experto en Gestión de Equipos Remotos. Diseña el protocolo de delegación para la tarea: [NOMBRE_TAREA]. 
1. Redacción del SOP (Standard Operating Procedure): Desglosa la tarea en 5-7 pasos inequívocos. Incluye ejemplos de 'Resultado Correcto' y 'Resultado Incorrecto'. 
2. Definición de Herramientas y Accesos: Especifica qué plataformas necesitará el colaborador y cómo gestionaremos la seguridad (Ej: LastPass/Bitwarden). 
3. Sistema de Checkpoints y Plazos: Establece cuándo queremos ver el progreso (Ej: Al 50% de la tarea) y cuál es el deadline final con un margen de seguridad. 
4. Guía de Resolución de Dudas (FAQ): Anticípate a las 3 preguntas más probables del colaborador y dales respuesta para evitar interrupciones asíncronas. 
5. Protocolo de Revisión y Feedback: Define cómo validaremos el trabajo recibido y qué canal usaremos para las correcciones (Ej: Comentarios en Notion/Loom).
```

### Fase 2: Ejecución, Ciclo de Ajuste y Delegación Total
... (Expansión técnica sobre el uso de la técnica de 'Shadowing Inverso' para validar que el colaborador ha entendido el proceso, la implementación de un proceso de 'Incremento Gradual de Responsabilidad' para construir confianza, y la monitorización del 'Tiempo Recuperado' por el titular para reinvertirlo en actividades de alto valor) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de libertad operativa.*

1.  **Trigger:** El titular identifica una tarea recurrente o masiva que supera su capacidad o no pertenece a su zona de genio.
2.  **Nodo de Creación de Activos de Delegación:** El sistema ayuda a capturar el flujo de trabajo (Video/Texto) y genera la documentación SOP inicial.
3.  **Nodo de Asignación y Onboarding:** Se selecciona al colaborador adecuado (IA o Humano) y se le entrega el paquete de información y accesos necesarios.
4.  **Nodo de Supervisión Asíncrona:** El sistema monitoriza los hitos de la tarea y gestiona las notificaciones de entrega o retraso.
5.  **Output:** Tarea completada con el estándar de calidad; tiempo del titular liberado; colaborador empoderado; SOP actualizado según el aprendizaje del ciclo.

---

## 7. Ejemplo Práctico: Agencia 'CreativeLaunch'
**Reto:** El director de 'CreativeLaunch' pasaba el 50% de su tiempo subiendo contenidos a las redes sociales de sus clientes, una tarea que le agotaba y le impedía buscar nuevos contratos. Tenía miedo de delegar por si "metían la pata con la marca".
**Acción v2.0:** Implementó Skill 250. Creó un SOP visual detallado en Notion con guías de tono, ejemplos de mejores publicaciones y un flujo de aprobación final mediante una simple señal en Slack.
**Resultados:** Delegó la tarea a un asistente virtual en 1 semana. El director recuperó 20 horas semanales. En el primer mes de delegación estructurada, cerró 2 nuevos clientes de alto valor que antes no podía atender, amortizando el coste del asistente en solo 3 días de trabajo recuperado.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
