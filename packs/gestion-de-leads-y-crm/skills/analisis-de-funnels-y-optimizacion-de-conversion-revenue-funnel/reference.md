# Referencia ampliada — Análisis de Funnels y Optimización de Conversión (Revenue Funnel Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de monitorización de rendimiento.*

1.  **Trigger:** Se alcanza un número significativo de sesiones o se detecta una desviación del >10% en la tasa de conversión habitual.
2.  **Nodo de Segmentación Automática:** El sistema desglosa los datos por dispositivo, navegador y procedencia para aislar el error.
3.  **Nodo de Alerta de Anomalía:** Si la caída se concentra en un paso específico, envía una alerta a Slack al equipo de Producto con los datos del fallo.
4.  **Nodo de Sugerencia de Mejora:** IA analiza el feedback cualitativo (encuestas o grabaciones) y propone 2 cambios de diseño o copy.
5.  **Output:** Dashboard actualizado con el impacto de la última optimización; visibilidad total del ROI de cada euro invertido.

---

## 7. Ejemplo Práctico: E-commerce de Moda
**Reto:** El 80% de los usuarios ponían productos en el carrito pero solo el 5% compraba.
**Acción v2.0:** El análisis de funnel detectó que la caída ocurría al pedir el código postal para calcular el envío. Se automatizó el cálculo por IP y se movió ese paso al final.
**Resultado:** La tasa de finalización de compra subió del 5% al 18% en un mes. Los ingresos se triplicaron sin aumentar el presupuesto en publicidad.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
