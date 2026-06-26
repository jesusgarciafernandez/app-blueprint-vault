# Referencia ampliada — MLOps (Machine Learning Operations & Lifecycle Management)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de resiliencia operativa.*

1.  **Trigger:** Registro de un nuevo modelo validado en el 'Model Registry' o detección de bajada de rendimiento en producción.
2.  **Nodo de Verificación y Empaquetado:** El sistema convierte el modelo (ej: .pth) en un contenedor Docker optimizado para el hardware de destino.
3.  **Nodo de Despliegue Controlado (Stage/Prod):** La IA se despliega inicialmente en un subconjunto de usuarios monitorizando métricas técnicas y de negocio.
4.  **Nodo de Monitorización de Inferencia:** Sensores en tiempo real miden latencia, consumo de memoria y concordancia del output con las expectativas humanas.
5.  **Output:** Servicio de IA estable y escalado; dashboard de salud del modelo y costes operativos generado para el humano.

---

## 7. Ejemplo Práctico: Predictor de Precios 'DynamicRent'
**Reto:** Su modelo de precios de alquiler fallaba cada vez que había un evento local no previsto (ej: un concierto) porque los datos de entrenamiento "se quedaban viejos" en días.
**Acción v2.0:** Implementaron MLOps (Skill 219). El sistema monitoriza el error de predicción cada hora y re-entrena el modelo automáticamente si el error supera el 5%.
**Resultado:** La precisión se mantiene estable independientemente de la estacionalidad, y el equipo técnico ha pasado de dedicar 10 horas semanales a despliegues manuales a solo supervisar el dashboard de automatización.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
