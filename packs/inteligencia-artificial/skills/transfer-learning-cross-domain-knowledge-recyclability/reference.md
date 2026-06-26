# Referencia ampliada — Transfer Learning (Cross-Domain Knowledge Recyclability)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Selección del "Donante" y Estrategia de Inserción
**Objetivo:** Elegir el modelo base que más sabe sobre algo parecido a nuestro reto.
1.  **Auditoría de Relevancia del Modelo Base:** IA ayuda a evaluar si un modelo entrenado en [DATOS_ORIGEN] tiene una representación interna útil para [TAREA_NUEVA].
2.  **Configuración del 'Head' de Clasificación:** Sustitución de la última capa del modelo pre-entrenado por una nueva estructura adaptada al número de clases del problema actual.

**Prompt Maestro de Transfer Learning:**
```text
Actúa como un Senior AI Architect y Experto en Eficiencia de Modelos. Diseña la estrategia de Transfer Learning para el reto [TAREA_NUEVA] usando el modelo base [NOMBRE_MODELO_BASE]. 
1. Análisis de Capas (Feature Extraction): Identifica hasta qué profundidad del modelo base congelaremos los pesos (Freezing) para mantener los extractores de características generales robustos. 
2. Diseño del Adaptador (Head): Propón la arquitectura de las nuevas capas superiores que añadiremos al final del modelo (Ej: Global Average Pooling -> Dropout -> Dense layer). 
3. Tasa de Aprendizaje Diferencial: Define por qué usaremos una tasa muy pequeña (Ej: 1e-5) para el cuerpo del modelo y una mayor (Ej: 1e-3) para el nuevo 'head' para no destruir el conocimiento previo. 
4. Estrategia de 'Warm-up': Diseña el proceso de introducción gradual de los datos nuevos para que los gradientes iniciales no desestabilicen los pesos heredados del modelo masivo. 
5. Protocolo de Evaluación de Transferencia: Define la métrica comparativa para demostrar que el modelo transferido supera en velocidad y precisión a un modelo entrenado desde cero.
```

### Fase 2: Ejecución, Descongelado Gradual y Validación
... (Expansión técnica sobre el uso de la técnica de 'Gradual Unfreezing' para ir haciendo el modelo más flexible capa a capa, la implementación de un proceso de 'Domain Adaptation' para ajustar el modelo a cambios sutiles en la distribución de datos y la monitorización de la 'Generalización' para asegurar que el modelo no se ha vuelto demasiado rígido tras la transferencia) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de herencia inteligente.*

1.  **Trigger:** Necesidad de un modelo de alta precisión pero con recursos limitados de datos o tiempo de computación.
2.  **Nodo de Descarga y Carga de Pesos:** El sistema descarga automáticamente el 'Pre-trained Model' y congela las capas fundamentales.
3.  **Nodo de Adaptación de la Arquitectura:** IA inyecta las capas superiores necesarias para la nueva tarea específica.
4.  **Nodo de Fine-tuning Supervisado:** Se entrena el modelo con el set de datos pequeño, ajustando solo las partes permitidas para maximizar la especialización.
5.  **Output:** Modelo optimizado listo para despliegue; métricas de ahorro de tiempo y energía generadas comparando con un entrenamiento base.

---

## 7. Ejemplo Práctico: Clasificador de Recambios 'AutoMatch'
**Reto:** Un taller necesitaba una app que identificara 500 tipos de bujías antiguas. Solo tenían 20 fotos de cada una, insuficiente para entrenar una IA desde cero.
**Acción v2.0:** Usaron Transfer Learning (Skill 218) con ResNet50. Congelaron el 80% de la red y solo entrenaron el clasificador final con sus fotos.
**Resultado:** En solo 2 horas de entrenamiento, lograron una precisión del 94%. El sistema ahora funciona en móviles baratos de los mecánicos, ahorrando horas de búsqueda en catálogos manuales.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
