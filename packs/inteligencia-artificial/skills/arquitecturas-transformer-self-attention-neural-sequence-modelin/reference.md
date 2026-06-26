# Referencia ampliada — Arquitecturas Transformer (Self-Attention & Neural Sequence Modeling)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Ingeniería del Grafo y Configuración de Atención
**Objetivo:** Definir la escala y la naturaleza del "cerebro" de la IA.
1.  **Definición de Hiperparámetros de Arquitectura:** IA ayuda a establecer el número óptimo de cabezas de atención, capas y dimensiones de embedding según el hardware disponible.
2.  **Configuración de Máscaras y Atenuación:** Diseño de cómo el modelo "mirará" al pasado (Causal mask) o al presente (Bidirectional) para cumplir su tarea.

**Prompt Maestro de Arquitecturas Transformer:**
```text
Actúa como un Senior AI Researcher y Arquitecto Jefe de Modelos Masivos. Diseña la arquitectura Transformer para el reto [TIPO_DE_DATO/TAREA]. 
1. Estructura de Capas: Define el número de bloques de Encoder/Decoder y el ratio de expansión en las capas 'Feed-Forward' para maximizar la capacidad de aprendizaje. 
2. Mecanismo de Atención: Propón el número de cabezas (Heads) y explica cómo gestionaremos el coste cuadrático de la atención en secuencias largas (Ej: Sparse Attention, RoPE). 
3. Representación de Posición: ¿Qué técnica de 'Positional Encoding' usaremos para que el modelo no pierda el orden de los datos y por qué (Ej: Senoidales vs Aprendidas)? 
4. Estrategia de Normalización: Establece si usaremos 'Pre-LN' o 'Post-LN' para asegurar la estabilidad del gradiente durante el entrenamiento de billones de parámetros. 
5. Protocolo de Eficiencia: Propón 2 técnicas de cuantización o poda (Pruning) para que el modelo resultante sea rápido en inferencia sin perder precisión crítica.
```

### Fase 2: Ejecución, Estabilización de Entrenamiento y Auditoría
... (Expansión técnica sobre el uso de la técnica de 'Gradient Clipping' para evitar explosiones, el análisis de la 'Atención Residual' para asegurar que la información fluye hasta las capas profundas y la monitorización de los pesos de la red para detectar 'cabezas de atención muertas' que no están aportando valor al razonamiento del modelo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de procesamiento de atención masiva.*

1.  **Trigger:** Entrada de una secuencia masiva de datos (Texto/Imagen/Audio) al sistema.
2.  **Nodo de Incrustación (Embedding) y Posición:** Los datos se convierten en vectores densos y se les inyecta la información de su posición relativa.
3.  **Nodo de Procesamiento de Atención:** Múltiples cabezas de atención extraen diferentes patrones de relación entre todos los elementos de la entrada en paralelo.
4.  **Nodo de Transformación No Lineal:** Las capas 'Feed-Forward' procesan la información de la atención para extraer características de alto nivel.
5.  **Output:** Representación contextualizada lista para la tarea final (Traducción/Generación/Clasificación); métricas de uso de memoria y GPU registradas.

---

## 7. Ejemplo Práctico: Traductor 'SwiftGlobal'
**Reto:** Su antiguo traductor basado en LSTMs (RNNs) traducía frases largas mezclando el significado y olvidando el sujeto al final de la frase.
**Acción v2.0:** Implementaron Arquitectura Transformer (Skill 212). El modelo ahora puede procesar documentos enteros de una sola vez, manteniendo la coherencia gramatical y técnica completa.
**Resultado:** La precisión en idiomas complejos subió un 40% y el sistema ahora puede traducir manuales técnicos de 500 páginas en una fracción del tiempo anterior con coherencia terminológica perfecta.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
