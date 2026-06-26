# Referencia ampliada — Gestión de E-commerce (Digital Retail & Ops Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de procesamiento de venta.*

1.  **Trigger:** El cliente completa el pago de un pedido en la tienda online.
2.  **Nodo de Verificación y Fraude:** El sistema cruza datos para asegurar que el pago es auténtico y el stock está realmente disponible.
3.  **Nodo de Orquestación de Almacén:** Envío automático de la orden de picking al almacén más cercano y generación de la etiqueta de transporte.
4.  **Nodo de Comunicación al Cliente:** Envío de recibo legal y enlace de seguimiento dinámico por SMS/WhatsApp.
5.  **Output:** Pedido enviado y registrado en contabilidad; el inventario se actualiza en todos los canales de venta simultáneamente.

---

## 7. Ejemplo Práctico: Marca de Cosmética 'Aha Baby'
**Reto:** Tenían un 80% de abandono de carrito en móvil porque el registro era demasiado largo y pedía el DNI obligatoriamente al principio.
**Acción v2.0:** Se activó el "Guest Checkout" con Apple Pay/Google Pay. Se redujo el formulario a 2 campos. Se enviaron notificaciones push de "Stock agotándose" a quienes dejaron el carrito.
**Resultado:** La tasa de conversión en móvil subió del 1.2% al 4.5% en un mes. Las ventas totales crecieron un 30% sin aumentar el gasto en publicidad.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
