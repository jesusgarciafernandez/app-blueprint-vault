# Referencia ampliada — Sistema de Encuestas NPS y Post-venta (Automated Feedback Loops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de captación y reacción al feedback.*

1.  **Trigger:** Finalización exitosa de un proceso clave (Ej: Entrega de pedido, Fin de suscripción anual).
2.  **Nodo de Envío de Micro-Survey:** El sistema manda la encuesta optimizada para móviles (1 sola pregunta + 1 comentario).
3.  **Nodo de Procesamiento de Respuesta:** IA categoriza el sentimiento y el tema de la respuesta abierta.
4.  **Nodo de Acción Resolutiva:** Si la nota es baja, se crea una tarea de "Rescate de Cliente" en HubSpot; si es alta, se le agradece y se le pide una reseña pública.
5.  **Output:** Flujo constante de inteligencia de mercado; reducción de puntos ciegos operativos y aumento de la fidelidad del cliente por sentirse escuchado.

---

## 7. Ejemplo Práctico: Suscripción de Software 'DesignTool'
**Reto:** No sabían por qué los clientes se iban tras pagar el primer año. Las encuestas anuales tenían una tasa de respuesta del 5%.
**Acción v2.0:** Implementaron el NPS automatizado a los 3, 6 y 11 meses. A los 3 meses detectaron que mucha gente tenía dudas con la facturación.
**Resultado:** Arreglaron el portal de facturación proactivamente. La tasa de respuesta subió al 32% (encuestas cortas). El Churn anual bajó un 12% al resolver dudas "latentes" detectadas a los 6 meses.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
