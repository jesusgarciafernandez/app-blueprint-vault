# Referencia ampliada — Chatbot Development & Conversational AI (AI Agent Orchestration)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de interacción del agente de IA.*

1.  **Trigger:** El usuario envía un mensaje a través de Web, WhatsApp o Widget.
2.  **Nodo de Procesamiento Semántico:** El LLM analiza la intención (Intent) y busca la información necesaria en la base de conocimientos propia (RAG).
3.  **Nodo de Ejecución de Acción:** Si la consulta requiere una acción, el bot llama a la API correspondiente y espera el resultado.
4.  **Nodo de Generación de Respuesta:** El bot redacta la respuesta final incorporando los datos obtenidos y manteniendo la personalidad definida.
5.  **Output:** Usuario satisfecho con respuesta inmediata y precisa; los datos de la interacción se guardan en el CRM para análisis futuro.

---

## 7. Ejemplo Práctico: Bot de Soporte para E-commerce 'EcoShop'
**Reto:** Tenían 200 correos al día preguntando "¿Dónde está mi pedido?". El equipo tardaba 24h en responder.
**Acción v2.0:** Crearon un agente en Voiceflow conectado a su base de datos de Shopify. El bot pedía el número de pedido y el email, y daba el estado del envío en tiempo real.
**Resultado:** El bot resolvió el 75% de las consultas de logística sin intervención humana. El tiempo de respuesta pasó de 24h a 2 segundos. La satisfacción del cliente subió un 30%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
