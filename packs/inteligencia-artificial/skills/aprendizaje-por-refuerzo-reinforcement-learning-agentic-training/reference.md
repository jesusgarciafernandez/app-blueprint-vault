# Referencia ampliada — Aprendizaje por Refuerzo (Reinforcement Learning & Agentic Training)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de evolución estratégica.*

1.  **Trigger:** Necesidad de optimizar un proceso de decisión complejo donde el humano no conoce la regla perfecta.
2.  **Nodo de Ejecución en Simulación (Rollout):** El agente ejecuta miles de episodios de prueba en un entorno controlado capturando (Estado, Acción, Recompensa).
3.  **Nodo de Actualización Core (Optimization):** La red neuronal del agente se ajusta para aumentar la probabilidad de las acciones que trajeron más recompensa.
4.  **Nodo de Evaluación de Rendimiento:** El sistema compara al agente actual con versiones previas para certificar que hay una mejora real y estable.
5.  **Output:** Agente entrenado incorporado al proceso operativo; log de recompensas y estrategias descubiertas disponible para el humano.

---

## 7. Ejemplo Práctico: Control Térmico 'PureEfficiency'
**Reto:** Gestionar el aire acondicionado de un centro de datos de 10 plantas era extremadamente costoso por la variabilidad de la temperatura exterior y la carga de los servidores.
**Acción v2.0:** Implementaron Aprendizaje por Refuerzo (Skill 211). El agente aprendió a pre-enfriar plantas antes de las horas pico de calor basándose en previsiones climáticas.
**Resultado:** Redujeron el consumo energético un 28% respecto al sistema de termostatos tradicional, logrando un ahorro anual de 2 millones de euros y una mayor vida útil de los equipos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
