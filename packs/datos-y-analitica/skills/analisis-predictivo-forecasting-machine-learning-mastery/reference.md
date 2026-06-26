# Referencia ampliada — Análisis Predictivo (Forecasting & Machine Learning Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de anticipación.*

1.  **Trigger:** Actualización diaria de la base de datos de transacciones o comportamiento de usuario.
2.  **Nodo de Preprocesamiento Automático:** El sistema limpia los nuevos datos y calcula las variables de entrada necesarias para el modelo.
3.  **Nodo de Inferencia por IA:** El modelo entrenado recibe los datos y genera una predicción (Ej: "Este usuario tiene un 85% de probabilidad de Churn").
4.  **Nodo de Acción Proactiva:** Si la predicción cruza un umbral crítico, se dispara una acción automática (Ej: Enviar cupón de descuento o alerta al gestor de cuenta).
5.  **Output:** Dashboard predictivo actualizado; intervención manual enfocada en prevenir el suceso antes de que ocurra.

---

## 7. Ejemplo Práctico: E-commerce 'FitGear'
**Reto:** Perdían el 20% de sus suscriptores cada mes y no sabían quién se iría hasta que ya habían cancelado.
**Acción v2.0:** Entrenaron un modelo de clasificación con los datos de actividad. La IA detectó que los usuarios que no entraban en la app durante 10 días tenían un 90% de probabilidad de baja.
**Resultado:** Implementaron un flujo que enviaba un email de contenido motivacional al día 8 de inactividad. El Churn se redujo un 15% en solo 2 meses.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
