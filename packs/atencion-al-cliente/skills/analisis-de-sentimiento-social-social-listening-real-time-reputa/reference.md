# Referencia ampliada — Análisis de Sentimiento Social (Social Listening & Real-Time Reputation)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de protección de reputación.*

1.  **Trigger:** El volumen de menciones negativas de la marca en X (Twitter) supera la media horaria en un 50%.
2.  **Nodo de Clasificación de Emergencia:** IA analiza los posts más virales para identificar si es un problema real del producto o un malentendido de comunicación.
3.  **Nodo de Notificación de Guerra (War Room):** El sistema abre un canal temporal en Slack con toda la información y convoca a los responsables de PR y Social Media.
4.  **Nodo de Respuesta Sugerida:** IA propone un mensaje oficial y una serie de respuestas personalizadas a los usuarios más influyentes.
5.  **Output:** Crisis contenida en las primeras 2 horas; la marca demuestra agilidad y transparencia, mejorando su imagen a pesar del incidente inicial.

---

## 7. Ejemplo Práctico: Fintech 'FastBank'
**Reto:** Un fallo en su app de 10 minutos provocó una oleada de "FastBank me ha robado mi dinero" en TikTok. El equipo de redes sociales estaba durmiendo.
**Acción v2.0:** El sistema detectó la anomalía de sentimiento, despertó al equipo y sugirió un video rápido del CTO explicando el fallo técnico mientras se solucionaba.
**Resultado:** El video explicativo fue más viral que las quejas. El sentimiento positivo subió al valorar los usuarios la "transparencia radical" de la empresa.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
