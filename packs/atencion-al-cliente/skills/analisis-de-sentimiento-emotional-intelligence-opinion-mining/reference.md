# Referencia ampliada — Análisis de Sentimiento (Emotional Intelligence & Opinion Mining)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de monitorización emocional.*

1.  **Trigger:** Llega un nuevo comentario, reseña o mensaje directo a la plataforma.
2.  **Nodo de Procesamiento NLP:** El sistema extrae el texto, el autor y la metainformación; el modelo de IA clasifica la polaridad y los aspectos.
3.  **Nodo de Lógica Reaccional:** Si el sentimiento es "Muy Negativo" (< 0.2), se dispara una alerta roja en Slack al equipo de Customer Success.
4.  **Nodo de Registro Histórico:** Se guardan los datos procesados en una base de datos vectorial para analizar tendencias semanales.
5.  **Output:** Dashboard de reputación actualizado en tiempo real; intervención humana inmediata en casos críticos de insatisfacción.

---

## 7. Ejemplo Práctico: Cadena de Hoteles 'Sun & Rest'
**Reto:** Recibían 500 reseñas a la semana en 10 idiomas. No sabían exactamente por qué bajaba su nota en Booking.
**Acción v2.0:** Implementaron un análisis por aspectos. La IA detectó que el 70% de las quejas negativas en el hotel de Marbella se referían específicamente al "tiempo de espera en el desayuno".
**Resultado:** Contrataron a dos camareros más para el desayuno. En un mes, el sentimiento positivo en las reseñas subió un 15% y la nota media en Booking pasó de 7.8 a 8.4.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
