# Referencia ampliada — IA Master (LLM Orchestration & RAG Ecosystem)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Arquitectura de la Solución Inteligente
**Objetivo:** Diseñar el "sistema nervioso" de la aplicación.
1.  **Selección del Motor de Razonamiento:** IA ayuda a elegir el modelo adecuado (Ej: Claude 3.5 para razonamiento complejo vs GPT-4o-mini para velocidad/coste).
2.  **Diseño del Pipeline de Conocimiento (RAG):** Definición de cómo se ingerirán, fragmentarán (chunking) e indexarán los datos de la base de conocimiento especializada.

**Prompt Maestro de IA Master (Architect Level):**
```text
Actúa como un Chief AI Architect y Senior AI Engineer. Diseña la solución de IA Master para el reto: [TAREA/PROYECTO]. 
1. Arquitectura de Orquestación: Propón el uso de LangChain/LangGraph y define los agentes necesarios (Ej: 'Ingestor', 'Auditor', 'Redactor'). 
2. Estrategia de RAG: Describe cómo vincularemos la base de datos vectorial [TIPO_DB] y qué técnica de 'Hybrid Search' usaremos para garantizar 0 alucinaciones. 
3. Definición de Herramientas (Toolsets): Lista las 3 APIs o funciones de código que los agentes deben manejar autónomamente para cumplir la misión. 
4. Gestión de Memoria: Define cómo el sistema guardará el progreso de la tarea para reanudarla si hay un fallo o una interrupción. 
5. Protocolo de Verificación Final: ¿Qué sistema de 'Self-Correction' aplicaremos para que la IA revise su propio output antes de mostrarlo al humano?
```

### Fase 2: Ejecución, Monitorización de Inferencia y Escalado
... (Expansión técnica sobre el uso de la técnica de 'Chain-of-Thought' para procesos de lógica profunda, la implementación de un proceso de 'Instruction Tuning' para adaptar el comportamiento a micro-tareas y la monitorización de la 'Deriva de Calidad' para asegurar que el sistema mantiene su precisión a lo largo del tiempo y con volúmenes crecientes de datos) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de inteligencia integral.*

1.  **Trigger:** Entrada de una solicitud compleja, evento de sistema o actualización de datos en el conocimiento base.
2.  **Nodo de Recuperación y Contextualización:** El sistema busca en la memoria vectorial e inyecta la "sabiduría local" necesaria en el prompt del modelo.
3.  **Nodo de Razonamiento y Planificación:** El Agente Maestro descompone la solicitud en pasos pequeños y decide qué herramientas invocar.
4.  **Nodo de Ejecución y Validación:** Las acciones se ejecutan (llamadas API, escritura de ficheros, cálculos) y el resultado se valida contra el objetivo original.
5.  **Output:** Solución terminada y entregada; el sistema de log registra el éxito y el consumo de tokens para optimización continua del ROI.

---

## 7. Ejemplo Práctico: Gestión Integral de Proyectos 'AutoTeam'
**Reto:** Un gestor de proyectos saturado con 50 canales de chat, 200 emails y 5 herramientas de gestión diferentes (Jira, Notion, Slack). No podía ver la foto global.
**Acción v2.0:** Implementaron IA Master (Skill 007). Un enjambre de agentes lee todos los canales, extrae los hilos de decisión, consulta los manuales de procedimientos (RAG) y prepara un resumen estratégico diario.
**Resultado:** El gestor ahora solo dedica 30 minutos al día a supervisar el "resumen inteligente". La IA incluso detecta retrasos potenciales antes de que ocurran analizando el tono de los mensajes, permitiendo una gestión proactiva y sin estrés.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
