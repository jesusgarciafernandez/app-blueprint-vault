# Referencia ampliada — Orquestación de Notificaciones Omnicanal (Omnichannel Master v2.0)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de pulso informativo.*

1.  **Trigger:** Ocurrencia de un evento en el backend, cambio de estado en la base de datos o activación de una campaña de marketing programada.
2.  **Nodo de Identificación y Preferencias:** El sistema busca al usuario, detecta sus canales activos y sus preferencias de notificación guardadas.
3.  **Nodo de Selección de Canal y Templating:** La IA selecciona el canal óptimo para la importancia del mensaje y genera el contenido personalizado usando la plantilla adecuada.
4.  **Nodo de Despacho y Registro (Audit Log):** El sistema envía el mensaje a través de la API del proveedor (FCM/Resend/Twilio) y registra la fecha e ID de envío.
5.  **Output:** Usuario informado por el canal correcto; historial de comunicación actualizado; métricas de entrega disponibles para optimización continua; integridad del sistema garantizada.

---

## 7. Ejemplo Práctico: El Marketplace 'UrgentBuy'
**Reto:** 'UrgentBuy' perdía ventas porque los usuarios no se enteraban a tiempo de que habían recibido una oferta por su producto. El Email se perdía entre otros correos y no tenían sistema de Push.
**Acción v2.0:** Implementaron Skill 004. Integraron FCM para Web Push en tiempo real. Ahora, cuando hay una oferta, se envía un Push inmediato al móvil del vendedor. Si en 15 minutos no ha clicado, el sistema dispara un Email transaccional recordatorio. Para ofertas de alto valor (>500€), se escala a SMS si no hay respuesta en 1 hora.
**Resultado:** La velocidad de cierre de ventas subió un 40%. Los usuarios reportan una sensación de "marketplace vivo" y eficaz. El coste de los SMS está compensado por las altas comisiones de las ventas de gran valor que ya no se pierden en el limbo de la bandeja de entrada.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
