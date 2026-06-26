# Referencia ampliada — Buscador Documental RAG (Specialized Manuals & Knowledge Retrieval)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de consulta experta.*

1.  **Trigger:** Pregunta técnica del usuario a través de un chat o interfaz de búsqueda.
2.  **Nodo de Transformación Vectorial:** El sistema convierte la pregunta en un vector matemático.
3.  **Nodo de Recuperación Semántica:** Se consultan los 'Top N' fragmentos de los manuales en la base de datos de conocimiento.
4.  **Nodo de Síntesis IA:** El modelo procesa la duda + los fragmentos y redacta una respuesta coherente, técnica y citada.
5.  **Output:** Respuesta experta entregada al usuario; el sistema guarda la dupla (Pregunta/Respuesta) para análisis de brechas de conocimiento futuro.

---

## 7. Ejemplo Práctico: Técnica de Mantenimiento 'GlobalWind'
**Reto:** Los técnicos de parques eólicos debían subir a los aerogeneradores con manuales de 10kg. Tardaban 1 hora en encontrar el par de apriete exacto de un tornillo específico.
**Acción v2.0:** Implementaron un Buscador RAG (Skill 205). El técnico pregunta por voz a su casco: "¿Cuál es el par de apriete del eje principal del modelo v90?". 
**Resultado:** La IA responde en 3 segundos: "750 Nm, según el Manual de Montaje v2.1, Pág. 142". El ahorro de tiempo fue del 95% y se eliminaron los errores por consulta de versiones obsoletas.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
