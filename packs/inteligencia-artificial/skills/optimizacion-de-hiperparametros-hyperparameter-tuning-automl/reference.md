# Referencia ampliada — Optimización de Hiperparámetros (Hyperparameter Tuning & AutoML)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Definición del Espacio de Búsqueda y Objetivo
**Objetivo:** Acotar el territorio de exploración inteligente.
1.  **Definición del Espacio de Hiperparámetros:** IA ayuda a sugerir rangos razonables (Ej: Learning rate entre 1e-5 y 1e-2 en escala logarítmica).
2.  **Selección de la 'Objective Function':** Redacción de la función que la IA intentará maximizar (Ej: F1-Score) o minimizar (Ej: Error Cuadrático Medio).

**Prompt Maestro de Optimización de Hiperparámetros:**
```text
Actúa como un Senior ML Engineer y Arquitecto de Rendimiento Algorítmico. Diseña el estudio de optimización para el modelo [NOMBRE_MODELO]. 
1. Espacio de Búsqueda (Search Space): Define los 5 parámetros clave a optimizar y sus rangos sugeridos (Categorical, Int, Log-float) para maximizar la exploración. 
2. Algoritmo de Búsqueda Sugerido: Justifica el uso de TPE (Tree-structured Parzen Estimator) o CMA-ES basándote en la complejidad del espacio de parámetros. 
3. Estrategia de 'Pruning' (Poda): Define en qué momento detendremos un experimento que va mal (Ej: MedianPruner) para liberar recursos para otros más prometedores. 
4. Validación Robusta: Configura una estrategia de 'K-Fold Cross-Validation' para asegurar que los mejores parámetros funcionan en diferentes subconjuntos de datos. 
5. Reporte de Importancia: Diseña la visualización final (Ej: Contour plot / Parallel Coordinate) que mostrará qué parámetros fueron los que realmente movieron la aguja del éxito.
```

### Fase 2: Ejecución, Monitorización de Pruebas y Reporte Final
... (Expansión técnica sobre el uso de la técnica de 'Multi-Objective Optimization' para equilibrar precisión y velocidad de inferencia, la implementación de un sistema de persistencia de resultados (SQLite/PostgreSQL) para no perder los experimentos si cae el sistema, y la auditoría de los mejores parámetros antes de pasarlos a producción para verificar su estabilidad ante variaciones mínimas) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de sintonía automática.*

1.  **Trigger:** Completada la arquitectura del modelo; la precisión preliminar no es satisfactoria.
2.  **Nodo de Lanzamiento de 'Trials' Paralelos:** El sistema lanza múltiples variantes del modelo con configuraciones de parámetros dictadas por el optimizador bayesiano.
3.  **Nodo de Monitorización y Poda (Pruning):** IA detecta experimentos mediocres en las primeras épocas y los mata instantáneamente para ahorrar GPU.
4.  **Nodo de Análisis de Superficie de Respuesta:** El optimizador procesa todos los resultados para proponer la combinación ganadora que maximiza la métrica objetivo.
5.  **Output:** 'Best Hyperparameters Set' generado y listo para el entrenamiento final a gran escala; reporte de importancia de parámetros entregado al humano.

---

## 7. Ejemplo Práctico: Recomendador 'VentaMax'
**Reto:** Su motor de recomendaciones daba siempre los mismos 3 productos. Cambiar los parámetros a mano era desesperante y no mejoraba la conversión.
**Acción v2.0:** Implementaron Optimización de Hiperparámetros (Skill 216) con Optuna. Lanzaron 200 experimentos sobre el factor de regularización y la tasa de aprendizaje.
**Resultado:** Encontraron una configuración que ni el equipo técnico había imaginado. El CTR (Click-Through Rate) subió un 22% y el tiempo de respuesta del modelo bajó un 15% gracias a un ajuste más eficiente de la red.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
