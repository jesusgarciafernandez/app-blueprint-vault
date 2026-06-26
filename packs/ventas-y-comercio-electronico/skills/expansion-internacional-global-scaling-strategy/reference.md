# Referencia ampliada — Expansión Internacional (Global Scaling Strategy)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de ventas transfronterizas.*

1.  **Trigger:** El sistema detecta una visita o pedido desde un país fuera del mercado principal (Detección por IP/Browser).
2.  **Nodo de Adaptación de Interfaz:** El sitio web cambia automáticamente a la moneda local, el idioma detectado y muestra los costes de envío y aduanas exactos para ese destino.
3.  **Nodo de Validación Legal/Fiscal:** El sistema comprueba si el producto es exportable a ese país y calcula los impuestos específicos que deben cobrarse en el checkout.
4.  **Nodo de Enrutamiento Logístico:** Tras el pago, el pedido se envía automáticamente al almacén más cercano al país de destino para minimizar el tiempo de entrega.
5.  **Output:** Pedido internacional procesado de forma transparente para el cliente; el negocio se internacionaliza sin aumentar la carga operativa manual.

---

## 7. Ejemplo Práctico: Marca de Cosmética Orgánica Española
**Reto:** Recibían pedidos de EE.UU. y México, pero los gastos de envío de 40€ y los 15 días de espera hacían que el 90% de los carritos se abandonaran.
**Acción v2.0:** Se integró un centro de cumplimiento en Miami. El sitio web mostraba "Envío Gratis a USA en 48h". Se habilitaron pagos vía Apple/Google Pay.
**Resultado:** Las ventas internacionales pasaron de representar el 2% al 35% del total en un año, convirtiéndose en el motor de crecimiento principal de la marca.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
