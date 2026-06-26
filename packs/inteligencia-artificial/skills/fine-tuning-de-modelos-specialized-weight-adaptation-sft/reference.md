# Referencia ampliada — Fine-tuning de Modelos (Specialized Weight Adaptation & SFT)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Ingeniería de Dataset y Selección de Estrategia
**Objetivo:** Preparar la "lección" perfecta para el modelo.
1.  **Auditoría de Calidad del Dataset:** IA ayuda a eliminar ejemplos contradictorios o de baja calidad del set de entrenamiento.
2.  **Configuración de Hiperparámetros de Adaptación:** Definición del rango de LoRA (Rank), Alpha y el 'Target Modules' (capas a ajustar).

**Prompt Maestro de Fine-tuning de Modelos:**
```text
Actúa como un Senior Machine Learning Engineer y Experto en LLM Fine-tuning. Diseña el proceso de especialización para el modelo [MODELO_BASE] sobre el dominio [DOMINIO_VERTICAL]. 
1. Preparación del Dataset: Define el formato ideal (Ej: Alpaca, ChatML) y propone una estrategia para generar 1.000 ejemplos sintéticos de alta calidad para cubrir lagunas de conocimiento. 
2. Configuración PEFT (LoRA): Establece el Rango (Rank) y Alpha óptimos para equilibrar la capacidad de aprendizaje y la estabilidad del modelo, evitando el 'catastrophic forgetting'. 
3. Estrategia de Evaluación: Diseña un set de 50 preguntas 'Benchmark' específicas del sector para comparar el modelo antes y después del fine-tuning. 
4. Optimización de Memoria: ¿Qué técnicas de cuantización (4-bit/8-bit) y de gradiente (Gradient Checkpointing) usaremos para que el entrenamiento quepa en una sola GPU de [VRAM_DISPONIBLE]? 
5. Protocolo de Despliegue: Define los pasos para 'fusionar' (Merge) los pesos de LoRA con el modelo base y exportar el resultado a formatos optimizados (GGUF/EXL2).
```

### Fase 2: Ejecución, Monitorización de Pérdida y Refinamiento
... (Expansión técnica sobre el uso de la técnica de 'Early Stopping' para evitar el sobreajuste a los datos de entrenamiento, la implementación de un proceso de 'Model Evaluation' mediante otros LLMs (LLM-as-a-judge) y la auditoría de las capacidades del modelo tras la fusión para asegurar que no ha perdido la lógica general mientras ganaba la especialidad vertical) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de adaptación experta.*

1.  **Trigger:** Disponibilidad de un nuevo dataset verificado de un dominio específico.
2.  **Nodo de Pre-procesado y Tokenización:** El sistema convierte el texto en el formato matemático exacto que el modelo necesita.
3.  **Nodo de Entrenamiento con PEFT:** Se ejecuta el ciclo de entrenamiento ajustando solo las capas de adaptación (LoRA Adapters) y guardando puntos de control (Checkpoints).
4.  **Nodo de Evaluación Comparativa:** IA lanza automáticamente el Benchmark diseñado para medir la mejora de precisión en el dominio.
5.  **Output:** Adaptador (LoRA) o Modelo Fusionado listo para producción; reporte de métricas de precisión y coste generado.

---

## 7. Ejemplo Práctico: Fintech 'LoanSmart'
**Reto:** Su asistente de riesgos basado en GPT-4 fallaba en interpretar las normativas bancarias locales de 2024 porque no estaban en su entrenamiento base y el prompt era demasiado largo y caro.
**Action v2.0:** Realizaron un Fine-tuning (Skill 214) de un modelo Llama-3 8B usando sus manuales internos.
**Resultado:** El modelo especializado superó en precisión a GPT-4 en su nicho, la latencia bajó de 10 a 2 segundos y el coste de API se redujo un 90% al usar infraestructura propia optimizada.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
