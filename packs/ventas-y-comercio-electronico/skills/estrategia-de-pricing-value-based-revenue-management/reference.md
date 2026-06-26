# Referencia ampliada — Estrategia de Pricing (Value-Based Revenue Management)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de optimización de ingresos.*

1.  **Trigger:** Cambio en el coste de adquisición (CAC), movimiento de precio de la competencia o cambio en el stock/disponibilidad.
2.  **Nodo de Análisis de Elasticidad:** El sistema calcula cómo afectaría un cambio del X% en el precio al volumen de ventas total basado en datos históricos.
3.  **Nodo de Propuesta de Ajuste:** IA sugiere el nuevo precio óptimo para maximizar el margen bruto (Revenue - Costes).
4.  **Nodo de Despliegue de Precios:** Actualización masiva de precios en la web, marketplace o CRM tras la validación humana.
5.  **Output:** Precios optimizados para el máximo beneficio; reporte de impacto en conversion rate y margen neto generado.

---

## 7. Ejemplo Práctico: SaaS de Edición de Vídeo Online
**Reto:** Tenían un precio plano de 20€/mes. Muchos usuarios se quejaban de que era caro para un uso puntual, y los profesionales decían que era demasiado barato (desconfiaban de su potencia).
**Acción v2.0:** Se crearon 3 Tiers: Free (Línea de tiempo limitada), Pro (30€/mes para editores frecuentes) y Pay-per-Render (5€ por vídeo para uso puntual).
**Resultado:** Los ingresos subieron un 60%. Capturaron al usuario ocasional que antes no pagaba y elevaron el ticket de los profesionales que buscaban más potencia, todo sin perder a nadie.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
