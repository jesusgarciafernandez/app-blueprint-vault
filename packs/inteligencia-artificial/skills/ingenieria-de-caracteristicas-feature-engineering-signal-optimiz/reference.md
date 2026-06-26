# Referencia ampliada — Ingeniería de Características (Feature Engineering & Signal Optimization)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Datos y Diseño de Señales
**Objetivo:** Identificar la riqueza oculta en los datos de origen.
1.  **Análisis de Correlación y Varianza:** IA ayuda a detectar variables redundantes o que no varían (ruido) para eliminarlas proactivamente.
2.  **Brainstorming de Variables de Negocio:** Redacción de una lista de 5 nuevas características que el modelo no tiene pero que el humano sabe que son predictivas (Ej: 'Víspera de festivo').

**Prompt Maestro de Ingeniería de Características:**
```text
Actúa como un Senior Data Scientist y Arquitecto de Features. Diseña el set de variables estratégicas para el problema: [DESCRIPCIÓN_PROBLEMA]. 
1. Limpieza y Transformación: Define cómo trataremos los valores faltantes (Imputación por media, mediana o KNN) y qué técnica de escalado usaremos (Standard vs Min-Max). 
2. Creación de Features de Dominio: Propón 3 variables calculadas que combinen datos existentes para dar más contexto (Ej: 'Ratio_Uso_Batería', 'Tendencia_Gasto_Últimos_30_días'). 
3. Codificación de Categorías: Determina si usaremos 'One-Hot Encoding' (pocos valores) o 'Target Encoding' (alta cardinalidad) para que la IA entienda las etiquetas de texto. 
4. Selección de Features (Filter methods): Diseña el test de importancia (Ej: Mutual Information) para quedarnos solo con el Top 20% de las variables más potentes. 
5. Protocolo de 'Data Leakage': Establece reglas para asegurar que el modelo no aprenda de variables "del futuro" que no conocerá en el momento de la predicción real.
```

### Fase 2: Ejecución, Validación de Significado y Reporte
... (Expansión técnica sobre el uso de la técnica de 'Polynomial Features' para capturar interacciones no lineales entre variables, la implementación de un proceso de 'Dimensionality Reduction' (Ej: PCA) para visualizar grupos de datos complejos, y la monitorización de la 'Feature Importance' para asegurar que el modelo no se obsesione con una sola variable ruidosa) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de refinado de señales.*

1.  **Trigger:** Entrada de nuevos datos brutos en el entorno de entrenamiento o inferencia.
2.  **Nodo de Limpieza y Normalización:** El sistema aplica automáticamente las reglas de imputación y escalado predefinidas de forma reproducible.
3.  **Nodo de Generación Dinámica de Features:** IA calcula las nuevas variables basadas en las fórmulas de dominio (ej: cálculos temporales o agregaciones).
4.  **Nodo de Selección y Poda (Pruning):** Se eliminan las variables con baja varianza o alta correlación cruzada para evitar el sobreajuste.
5.  **Output:** 'Model-Ready Feature Set' estructurado; informe de calidad del dato y ranking de importancia de las variables generado.

---

## 7. Ejemplo Práctico: Mantenimiento Preventivo 'FlySafe'
**Reto:** Un sistema de aerolínea registraba miles de logs de temperatura de motores. Usar la temperatura directa no predecía fallos, ya que la temperatura sube naturalmente al despegar.
**Acción v2.0:** Aplicaron Ingeniería de Características (Skill 215). Crearon la variable "Desviación vs Promedio de Flota en misma altitud y carga". 
**Resultado:** Esta nueva "señal inteligente" permitió detectar averías 10 horas antes de que ocurrieran, algo imposible con los datos crudos. La precisión de las alertas subió un 35%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
