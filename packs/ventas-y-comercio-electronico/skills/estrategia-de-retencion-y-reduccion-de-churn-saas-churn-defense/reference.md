# Referencia ampliada — Estrategia de Retención y Reducción de Churn (SaaS Churn Defense)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de defensa de ingresos.*

1.  **Trigger:** El sistema detecta una señal de riesgo (Ej: Un usuario con plan 'Enterprise' no ha completado el onboarding tras 15 días).
2.  **Nodo de Clasificación de Riesgo:** Se asigna un Health Score bajo y se notifica al Customer Success Manager (CSM) por Slack.
3.  **Nodo de Acción Automatizada:** Se dispara un email personalizado con un video-tutorial o una invitación a una consultoría gratuita "1:1 de éxito".
4.  **Nodo de Monitorización de Respuesta:** Si el cliente vuelve a la plataforma, se marca como "Rescatado". Si no, se escala a la dirección comercial.
5.  **Output:** Tasa de Churn controlada; el equipo sabe exactamente dónde poner fuego para salvar las cuentas más valiosas.

---

## 7. Ejemplo Práctico: SaaS de Facturación 'SimpleBill'
**Reto:** Perdían el 5% de sus clientes al mes (Churn muy alto). Los clientes decían que el software era "difícil de configurar".
**Acción v2.0:** Implementaron un trigger: si un usuario no subía su logo en las primeras 24h, recibía un email con el asunto: "¿Te lo subo yo?". Si no entraban en 10 días, recibían un cupón para una sesión de 15min de configuración enviada por el propio CEO (automatizado).
**Resultado:** El Churn bajó del 5% al 1.8% en tres meses. El LTV medio por cliente aumentó un 40% al durar más meses suscritos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
