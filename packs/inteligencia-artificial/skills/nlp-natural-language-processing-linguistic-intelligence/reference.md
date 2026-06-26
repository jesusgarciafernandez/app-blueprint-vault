# Referencia ampliada — NLP (Natural Language Processing & Linguistic Intelligence)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de entendimiento verbal.*

1.  **Trigger:** Entrada de texto no estructurado desde un archivo, email, chat o base de datos.
2.  **Nodo de Normalización y Limpieza:** El sistema ajusta el texto, elimina ruido visual y prepara los tokens para la red neuronal.
3.  **Nodo de Inferencia Semántica (Modelos):** La IA procesa el texto en capas, identificando gramática, entidades y sentimientos predominantes.
4.  **Nodo de Estructuración de Datos:** IA convierte los hallazgos lingüísticos en un formato persistente (Tabla SQL o JSON) útil para el negocio.
5.  **Output:** Resumen y extracción de datos enviados al humano; alertas activadas ante detección de sentimientos críticos o información URGENTE.

---

## 7. Ejemplo Práctico: Moderación 'SafeCommunity'
**Reto:** Un foro con 100.000 mensajes diarios no podía ser moderado por humanos. Los filtros de palabras prohibidas eran fáciles de saltar usando símbolos o juegos de palabras.
**Action v2.0:** Implementaron NLP (Skill 221). Una IA analiza el "sentimiento y toxicidad semántica" de cada mensaje, no solo las palabras sueltas.
**Resultado:** La tasa de acoso bajó un 90%. El sistema ahora detecta la intención agresiva incluso si no se usan insultos directos, avisando instantáneamente a los moderadores humanos para que tomen la decisión final.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
