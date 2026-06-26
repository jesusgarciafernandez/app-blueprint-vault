# Referencia ampliada — Usability Testing, Validación Empírica y Análisis de Fricción

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de procesamiento de tests automatizada.*

1.  **Trigger:** Finalización de 10 sesiones de test no moderado en Maze para una nueva App de fitness.
2.  **Nodo de Análisis de Frustración IA:** El sistema analiza los 'Miss-clicks' y el tiempo de parálisis del ratón en cada pantalla.
3.  **Nodo de Transcripción y Sentimiento:** IA procesa el audio de los usuarios pensando en voz alta y agrupa las quejas por temática (ej: "Confusión con el precio").
4.  **Nodo de Clasificación de Severidad:** El sistema identifica que el 80% falló en la misma tarea crítica y lo marca como prioridad "Bloqueante".
5.  **Output:** Dashboard resumen con la puntuación de usabilidad (User Experience Score) y una lista de 3 cambios de diseño que resolverían el 90% de los problemas detectados.

---

## 7. Ejemplo Práctico: App de Reserva de Pistas de Pádel
**Reto:** Los usuarios se quejaban de que la App era "difícil", pero el diseño era estéticamente impecable.
**Acción v2.0:** Se hizo un test de usabilidad moderado. Se descubrió que la gente buscaba el botón de "Guardar" arriba, pero estaba oculto abajo por el teclado. También confundían el icono de "Filtro" con el de "Descarga".
**Resultado:** Se movió el botón y se cambió el icono por texto. La tasa de éxito en la reserva subió del 50% al 95% en la siguiente iteración.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
