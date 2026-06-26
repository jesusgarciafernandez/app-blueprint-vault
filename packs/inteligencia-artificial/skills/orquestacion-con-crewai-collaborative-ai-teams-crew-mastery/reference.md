# Referencia ampliada — Orquestación con CrewAI (Collaborative AI Teams & Crew Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Diseño de la 'Tripulación' (The Crew)
**Objetivo:** Definir quién hace qué y en qué orden dentro del equipo.
1.  **Mapeo de Roles y Perfiles:** IA ayuda a diseñar el 'Backstory' de cada agente para que "sienta" su especialidad (Ej: "Eres un Auditor Senior con ojo para el detalle").
2.  **Definición de Tareas y Dependencias:** Establecimiento de qué agente necesita el output de quién para comenzar su trabajo.

**Prompt Maestro de Orquestación con CrewAI:**
```text
Actúa como un Senior Agent Orchestrator y Experto en CrewAI. Diseña la tripulación para la misión: [DESCRIPCIÓN_MISIÓN]. 
1. Define los Agentes: Crea 3 agentes con su Rol, Goal y un Backstory potente que asegure la especialización (Investigador, Estratega, Creador). 
2. Diseña las Tareas: Define la 'Task description' y el 'Expected output' para cada una, asegurando que la salida sea estructurada (JSON/Markdown). 
3. Selección de Herramientas (Tools): ¿Qué herramientas específicas (Búsqueda web, Lectura de archivos, API custom) debe manejar cada agente? 
4. Configuración del Proceso: ¿Sugerirías un proceso 'Sequential' o un 'Manager LLM' para supervisar la calidad de las entregas? Justifica el porqué. 
5. Ejecución en Python: Genera el código base en Python para instanciar la Crew, los agentes y lanzar la misión (crew.kickoff()).
```

### Fase 2: Ejecución, Monitorización de Logs y Ajuste Táctico
... (Expansión técnica sobre el uso de la técnica de 'Self-Correction' donde los agentes piden una segunda opinión a sus compañeros, la monitorización de los logs de ejecución para detectar bucles de razonamiento y la implementación de sistemas de 'Memory' de la Crew para que recuerden hallazgos entre ejecuciones de la misma misión) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de trabajo en equipo digital.*

1.  **Trigger:** Recepción de un objetivo complejo que requiere múltiples pasos y especialidades.
2.  **Nodo de Orquestador CrewAI:** El sistema instancia la Crew y asigna la primera tarea al agente correspondiente basándose en el orden definido.
3.  **Nodo de Ejecución y Colaboración:** Los agentes ejecutan sus tareas, consultan herramientas y pasan la información procesada al siguiente eslabón.
4.  **Nodo de Auditoría y Consolidación:** Un agente supervisor (o el proceso gestionado) verifica que el resultado final cumple con todas las premisas.
5.  **Output:** Entregable complejo terminado; el sistema apaga la tripulación y guarda el log de "Aprendizaje del Equipo" para futuras misiones similares.

---

## 7. Ejemplo Práctico: Consultoría 'DataInsight'
**Reto:** Analizar 20 informes de sostenibilidad de la competencia y generar un resumen ejecutivo comparativo. Un consultor humano tardaba 3 días.
**Acción v2.0:** Implementaron una Crew (Skill 201). Un agente 'Lector' extraía datos, un agente 'Analista' buscaba discrepancias y un agente 'Writer' redactaba el reporte final.
**Resultado:** El reporte se generó en 8 minutos. La calidad del análisis fue superior al humano al no "cansarse" de leer miles de tablas numéricas. El consultor ahora solo revisa el análisis final para añadir el "toque estratégico".

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
