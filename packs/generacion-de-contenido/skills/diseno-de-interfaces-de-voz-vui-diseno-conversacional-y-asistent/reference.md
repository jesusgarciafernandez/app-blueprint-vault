# Referencia ampliada — Diseño de Interfaces de Voz (VUI), Diseño Conversacional y Asistentes IA

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de procesamiento de voz automatizada.*

1.  **Trigger:** Un usuario dice "Hola, quiero pedir una pizza margarita" a su altavoz inteligente.
2.  **Nodo de ASR (Speech-to-Text):** El sonido se convierte en texto en milisegundos.
3.  **Nodo de NLU (Comprensión de Intención):** El sistema identifica la intención (`order_food`) y la entidad (`pizza_type: margarita`).
4.  **Nodo de Gestión de Diálogo:** IA comprueba si falta información (ej: tamaño). Si falta, activa el nodo "Pregunta de aclaración".
5.  **Output (TTS):** El asistente responde en milisegundos: "Perfecto, una margarita. ¿De qué tamaño la prefieres, mediana o familiar?".

---

## 7. Ejemplo Práctico: Asistente para Recetas de Cocina
**Reto:** Los usuarios manchaban el móvil al intentar pasar de paso en una receta mientras cocinaban.
**Acción v2.0:** Se diseñó una interfaz de voz que permite avanzar, retroceder y preguntar cantidades ("¿Cuánta harina era?") sin tocar nada. El asistente usa un tono cercano y espera a que el usuario diga "Siguiente" para continuar.
**Resultado:** La tasa de abandono de recetas en medio de la cocción bajó un 60% y la satisfacción del usuario ("sentirse como un chef") subió notablemente.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
