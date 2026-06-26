# Referencia ampliada — Arquitectura de Experiencia de Usuario para Agentes IA (Agentic UX)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de orquestación de la experiencia agéntica.*

1.  **Trigger:** El usuario introduce una instrucción compleja de múltiples pasos.
2.  **Nodo de Segmentación de Tareas:** La IA desglosa el objetivo en 5 subtareas y las muestra en la interfaz (Transparencia).
3.  **Nodo de Ejecución con Feedback:** Mientras se ejecuta cada paso, se envía un mensaje vía Webhook para actualizar el estado visual del usuario en tiempo real.
4.  **Nodo de Alerta de Incertidumbre:** Si la IA detecta una ambigüedad, dispara un "Human-in-the-loop" bloqueando la ejecución hasta que el usuario aclare el punto.
5.  **Output:** Tarea completada con informe de trazabilidad, permitiendo al usuario auditar qué hizo la IA y por qué.

---

## 7. Ejemplo Práctico: Agente de Inversión Inmobiliaria
**Reto:** Los usuarios no se fiaban de una IA que decía "Invierte en este piso".
**Acción v2.0:** Se rediseñó la UX para mostrar los 20 factores analizados (barrio, precio m2, rentabilidad, etc.) en un flujo visual. Si el dato era antiguo, la IA ponía un icono de "Alerta de Confianza: Datos de hace 6 meses".
**Resultado:** La tasa de uso de la herramienta subió un 80% porque el usuario dejó de sentir que era una jugada de azar y empezó a sentir que tenía un analista junior muy eficiente reportándole datos procesados.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
