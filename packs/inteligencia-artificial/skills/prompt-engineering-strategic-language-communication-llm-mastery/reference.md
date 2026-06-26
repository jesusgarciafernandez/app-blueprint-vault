# Referencia ampliada — Prompt Engineering (Strategic Language Communication & LLM Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de comunicación inteligente.*

1.  **Trigger:** Necesidad de que una IA realice una tarea técnica o creativa con estándares de calidad profesional.
2.  **Nodo de Selección de Template:** El sistema carga el prompt maestro optimizado para esa categoría específica de tarea.
3.  **Nodo de Inyección de Semillas Dinámicas:** IA rellena los huecos del prompt con los datos frescos del usuario o del sistema actual.
4.  **Nodo de Ejecución y Validación de Formato:** El modelo genera la respuesta y un sensor automático verifica si cumple las restricciones de formato (ej: "¿Es un JSON válido?").
5.  **Output:** Resultado final impecable entregado al humano o al siguiente sistema; log de tokens y calidad guardado para auditoría.

---

## 7. Ejemplo Práctico: Generador de Blueprints 'ProDraft'
**Reto:** Una empresa quería que la IA diseñara planos de arquitectura en texto, pero la IA mezclaba metros con pies y a veces olvidaba incluir los baños.
**Acción v2.0:** Diseñaron un Prompt Maestro (Skill 222) con una estructura de "Auditor Interno". El prompt obligaba a la IA a hacer un checklist de requisitos ANTES de generar el diseño.
**Resultado:** Los errores se eliminaron por completo. El sistema ahora genera 50 diseños por hora con una coherencia total, permitiendo a los arquitectos centrarse en el diseño estético en lugar de corregir errores de medida básicos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
