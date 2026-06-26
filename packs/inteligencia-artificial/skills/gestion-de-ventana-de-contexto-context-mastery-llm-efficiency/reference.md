# Referencia ampliada — Gestión de Ventana de Contexto (Context Mastery & LLM Efficiency)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Información y Estrategia de Carga
**Objetivo:** Decidir qué información es 'Núcleo' y qué es 'Accesorio'.
1.  **Identificación de Contexto Estático:** IA ayuda a separar las instrucciones fijas (System Prompt) que pueden ser cacheadas.
2.  **Diseño del Pipeline de Recuperación:** Definición de cómo el sistema buscará la pieza exacta de información necesaria para responder cada duda.

**Prompt Maestro de Gestión de Contexto (Context Mastery):**
```text
Actúa como un Senior LLM Engineer y Experto en Optimización de Contexto. Analiza el siguiente set de información [INFO/TAREA]. 
1. Crea el Mapa de Contexto: Divide la información en (A) Instrucciones Core, (B) Datos de Soporte Críticos y (C) Ruido eliminable. 
2. Diseña la Estrategia de Compresión: ¿Cómo podemos resumir los datos de soporte sin perder entidades clave o valores numéricos? 
3. Implementación de Context Caching: Identifica qué parte del prompt será idéntica en el 80% de las llamadas para marcarla como 'Cacheable'. 
4. Lógica de Recuperación (RAG): Propón los metadatos de búsqueda para que el modelo recupere solo los [N] párrafos más relevantes para el usuario. 
5. Test de 'Atención': Diseña una prueba para verificar que el modelo no ignora información enviada en la parte central del contexto optimizado.
```

### Fase 2: Ejecución, Monitorización y Acción
... (Expansión técnica sobre el uso de la técnica de 'Ranking' para re-ordenar los fragmentos recuperados por relevancia semántica, la implementación de buffers de memoria rodante (Sliding Window) para mantener el histórico de chat sin desbordar el límite y la monitorización de la tasa de 'Context Recall' para asegurar que la IA no alucina por falta de datos) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de optimización de memoria.*

1.  **Trigger:** Entrada del usuario que requiere contexto histórico o documental.
2.  **Nodo de Recuperación Inteligente:** El sistema consulta la base de conocimiento o la memoria vectorial y extrae solo lo relevante para la pregunta actual.
3.  **Nodo de Compresión y Formateo:** IA ajusta los fragmentos recuperados para ocupar el mínimo de tokens posible manteniendo el significado.
4.  **Nodo de Inyección de Contexto en LLM:** Se construye el prompt final inyectando el contexto dinámico y la llamada a las partes cacheadas del sistema.
5.  **Output:** Respuesta precisa y coherente; el sistema de monitorización registra el consumo de tokens y la efectividad de la recuperación.

---

## 7. Ejemplo Práctico: Bufete de Abogados 'LexIA'
**Reto:** Necesitaban analizar 50 precedentes legales (3.000 páginas) para un caso nuevo. Al pegarlo todo en el chat, la IA empezaba a confundir nombres de jueces y fechas.
**Acción v2.0:** Implementaron Gestión de Contexto. Cachearon las leyes fundamentales y usaron RAG para inyectar solo los 3 precedentes más similares al caso actual en cada pregunta.
**Resultado:** La precisión subió del 65% al 98%. El coste de los análisis bajó un 60% al no reenviar las 3.000 páginas en cada interacción. La IA ahora "razona" mejor con menos distracciones.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
