# Referencia ampliada — RAG (Retrieval-Augmented Generation & Contextual AI)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Ingesta, Fragmentación y Vectorización
**Objetivo:** Crear el mapa de conocimiento que la IA podrá "leer".
1.  **Auditoría de Fuentes:** IA ayuda a priorizar qué documentos son críticos y deben ser indexados.
2.  **Diseño del Chunking Strategy:** Selección del tamaño de fragmento (Ej: 500 tokens con 10% de solapamiento) para no perder el contexto de las frases.

**Prompt Maestro de Implementación RAG (Knowledge Linker):**
```text
Actúa como un Senior AI Solution Architect y Experto en Retrieval-Augmented Generation. Diseña el pipeline de RAG para: [DESCRIPCIÓN_DATASET/DOMINIO]. 
1. Estrategia de Chunking: ¿Cómo dividirías los documentos (Ej: por párrafos, encabezados, o tamaño fijo) para maximizar la coherencia según [TIPOLOGÍA_DOCS]? 
2. Selección de Modelos: Propón el modelo de Embedding y el LLM de síntesis ideal, justificando la relación entre calidad de recuperación y coste de tokens. 
3. Arquitectura Vectorial: Diseña el esquema de metadatos (Metadata) que guardaremos junto a los vectores para poder filtrar por fecha, autor o categoría. 
4. Pipeline de Recuperación: Describe cómo manejaremos las consultas del usuario para transformarlas en vectores (Query Embedding) y cómo seleccionaremos los 'K' fragmentos más relevantes. 
5. Protocolo Anti-Alucinación: Redacta las 'Instrucciones de Sistema' que obliguen a la IA a decir 'No lo sé' si la información no está en el contexto recuperado.
```

### Fase 2: Ejecución, Evaluación del 'Retrieval' y Re-ranking
... (Expansión técnica sobre el uso de la técnica de 'Query Expansion' donde la IA genera variantes de la pregunta del usuario para buscar mejor, la implementación de un proceso de 'Re-ranking' con modelos como Cohere para ordenar los resultados por relevancia lingüística real y la monitorización de la 'Fidelidad de Respuesta' usando métricas como RAGAS) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de memoria contextual.*

1.  **Trigger:** Recepción de una consulta que requiere conocimiento específico no contenido en el entrenamiento base del modelo.
2.  **Nodo de Transformación Vectorial (Encoding):** El sistema convierte la pregunta del usuario en un vector numérico multienfoque.
3.  **Nodo de Búsqueda de Similitud:** La base de datos vectorial identifica los fragmentos de texto con la distancia semántica más corta a la pregunta.
4.  **Nodo de Generación de Respuesta Contextual:** El LLM recibe la pregunta + los fragmentos recuperados y redacta la respuesta citando las fuentes.
5.  **Output:** Respuesta precisa y verificable entregada al usuario; feedback de relevancia guardado para ajustar los pesos del buscador.

---

## 7. Ejemplo Práctico: Bufete de Abogados 'LexBot'
**Reto:** Los abogados tardaban días en revisar jurisprudencia buscando casos similares a los actuales en una base de datos de 50.000 sentencias.
**Acción v2.0:** Implementaron RAG (Skill 226). El sistema ahora permite preguntar "¿Hay sentencias previas sobre reclamación de vicios ocultos en naves industriales de más de 20 años?".
**Resultado:** El sistema recupera los 5 casos más parecidos en 3 segundos, resume los puntos clave de cada uno y enlaza al PDF original. La productividad del equipo de investigación aumentó un 500%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
