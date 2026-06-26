# Referencia ampliada — Patrones de Diseño Agénticos (Agentic Design Patterns & Robust AI)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Selección del Patrón y Diseño del Flujo
**Objetivo:** Elegir la estructura de razonamiento que mejor resuelve el problema.
1.  **Diagnóstico de la Tarea:** IA ayuda a determinar si el reto requiere crítica interna (Reflexión) o coordinación de especialistas (Multi-agente).
2.  **Diseño de los Nodos de Control:** Definición de qué sucede entre una llamada y la siguiente (Ej: "Si el código falla, vuelve al nodo de edición").

**Prompt Maestro de Patrones Agénticos (Agentic Design):**
```text
Actúa como un Senior AI Architect y Experto en Agentic Workflows. Diseña el sistema autónomo para [MISIÓN/TAREA]. 
1. Selección de Patrón: ¿Usaremos Reflexión, Planificación o Multi-Agente? Justifica por qué esta estructura es la más robusta para este caso. 
2. Diseño del 'Loop' de Mejora: Define los criterios que el agente usará para auto-evaluar su trabajo (Rúbrica de crítica interna). 
3. Definición de Herramientas (Tools): Lista las habilidades externas que el agente debe invocar y cómo manejaremos una respuesta de error del software. 
4. Punto de Escalamiento Humano: Define la 'Condición de Parada' en la que el agente debe dejar de iterar y pedir ayuda al humano (Ej: Tras 3 intentos fallidos). 
5. Esquema de Salida (Output Schema): Genera el modelo Pydantic o JSON que asegure que el resultado final sea estructurado y validable.
```

### Fase 2: Implementación, Calibración y Red Teaming
... (Expansión técnica sobre el uso de la técnica de 'Self-Consistency' para votar entre múltiples caminos de razonamiento, la implementación de límites de recursividad (Max Loops) para evitar costes infinitos y la creación de tests de 'Robustez Agéntica' donde se introducen fallos a propósito para ver si el patrón de diseño es capaz de recuperarse solo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de razonamiento iterativo.*

1.  **Trigger:** Recepción de una misión compleja de larga duración.
2.  **Nodo de Planificador (Planner):** IA descompone la misión en una lista jerárquica de subtareas ejecutables.
3.  **Nodo de Ejecución y Reflexión:** El agente realiza la primera subtarea, revisa el resultado y, si es necesario, vuelve a ejecutar con correcciones.
4.  **Nodo de Verificación de Hitos:** Un proceso supervisor valida que el paso actual es correcto antes de permitir el avance al siguiente punto del plan.
5.  **Output:** Resultado final verificado y consolidado; el sistema genera un informe del proceso de "Pensamiento" seguido para auditoría humana.

---

## 7. Ejemplo Práctico: Agencia de Traducción 'ContextTrans'
**Reto:** Traducir libros técnicos de 400 páginas manteniendo la coherencia de términos complejos. Un traductor de IA estándar (GPT) cometía errores de glosario a partir de la página 50.
**Acción v2.0:** Implementaron un Patrón de Reflexión. Un agente traducía el capítulo, otro comparaba los términos con el "Glosario de Oro" y, si encontraba una discrepancia, obligaba al primero a re-traducir el párrafo.
**Resultado:** La calidad fue idéntica a la traducción humana experta. El sistema se auto-corrigió en más de 200 puntos críticos sin intervención del supervisor, que solo validó el resultado final impecable.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
