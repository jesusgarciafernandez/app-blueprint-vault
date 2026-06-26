# Referencia ampliada — Síntesis Inteligente de Sesiones (Meeting Summarization & Insights)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Captura y Configuración del Analista IA
**Objetivo:** Asegurar que la entrada de audio es perfecta y el modelo sabe qué buscar.
1.  **Optimización del Hardware/Software de Audio:** IA ayuda a diagnosticar la calidad de la entrada de audio para minimizar el WER (Word Error Rate).
2.  **Definición del 'Template' de Resumen:** Diseño de la estructura de reporte que necesita la organización (Ej: Formato Ejecutivo vs. Formato Técnico).

**Prompt Maestro de Síntesis (Insight Engineer):**
```text
Actúa como un Senior Operations Analyst y Experto en NLP. Procesa la transcripción adjunta de la reunión sobre [TEMA_REUNIÓN]. 
1. Resumen Ejecutivo (TL;DR): Redacta un párrafo de 3 líneas con el impacto principal de la sesión. 
2. Bloque de Decisiones: Enumera los acuerdos cerrados inequívocamente (Ej: "Se aprueba el presupuesto de X"). 
3. Tabla de Action Items: Extrae las tareas, asígnalas a una persona y define la fecha límite basándote en el contexto de la charla. 
4. Análisis de Temas Calientes: Identifica puntos de fricción o temas que se quedaron sin resolver para la próxima agenda. 
5. Verbatims de Valor: Selecciona las 3 citas más importantes que reflejan la visión estratégica del grupo.
```

### Fase 2: Ejecución, Distribución y Auditoría de Compromisos
... (Expansión técnica sobre el uso de la técnica de 'Speaker Diarization' para identificar quién dijo qué, la implementación de un proceso de 'Auto-tagging' para clasificar resúmenes por proyecto, y la monitorización de la 'Tasa de Conversión de Ideas a Tareas' para asegurar la productividad post-reunión) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de claridad duradera.*

1.  **Trigger:** El sistema detecta el inicio de una videollamada programada o la activación manual de un grabador de voz.
2.  **Nodo de Captura y Transcripción:** Un agente recolecta el audio en tiempo real y genera el texto literal (STT).
3.  **Nodo de Procesamiento Semántico (AI Analyst):** El sistema aplica prompts especializados para limpiar el ruido (muletillas, saludos) y extraer la estructura de valor.
4.  **Nodo de Distribución Multicanal:** El resumen se envía por email, se publica en Slack y se crea una página en la base de conocimiento del proyecto.
5.  **Output:** Memoria de reunión disponible; tareas creadas en el backlog; equipo notificado; historial de decisiones actualizado y buscable.

---

## 7. Ejemplo Práctico: Startup 'AgileMind'
**Reto:** En 'AgileMind' tenían 10 reuniones de sprint al día. Los desarrolladores se quejaban de que "perdía el hilo" de lo acordado y los Project Managers pasaban 3 horas al día redactando actas que nadie leía.
**Acción v2.0:** Implementaron Skill 254. Instalaron un bot de IA que asiste a todas las reuniones de Zoom. Al terminar, envía un resumen de 2 minutos de lectura a Slack con los links a las nuevas tareas creadas directamente en Jira.
**Resultado:** Se eliminó el trabajo de redacción manual de actas. La alineación técnica subió un 40% porque los devs tienen el resumen visual al instante. El tiempo de 'context switching' se redujo, permitiendo más horas de código real.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
