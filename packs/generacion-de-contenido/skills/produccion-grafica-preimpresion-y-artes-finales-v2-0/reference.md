# Referencia ampliada — Producción Gráfica, Preimpresión y Artes Finales (v2.0)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control de calidad para imprenta.*

1.  **Trigger:** El diseñador exporta el PDF final para su envío.
2.  **Nodo de Preflight Automático:** IA analiza el PDF buscando imágenes de baja resolución, colores RGB incrustados o fuentes no trazadas/incrustadas.
3.  **Nodo de Corrección de Negro:** El sistema aplica automáticamente "Sobreimpresión de Negro" a los textos pequeños para evitar errores de registro en prensa.
4.  **Nodo de Generación de Informe de Error:** Si hay problemas críticos (resolución < 200 DPI), el sistema bloquea el envío y avisa al diseñador con la ubicación exacta del fallo.
5.  **Output:** Archivo validado y certificado listo para imprenta, entregado con un sello de calidad técnica.

---

## 7. Ejemplo Práctico: Catálogo de Moda Otoño/Invierno
**Reto:** En la última tirada, los colores de los abrigos salieron oscuros y los textos negros tenían un aura blanca alrededor. Perder 5000 catálogos costó miles de euros.
**Action v2.0:** Se implementó un flujo de producción riguroso: perfiles de color para papel estucado mate, sobreimpresión de negros obligatoria y marcas de registro milimétricas.
**Resultado:** Los catálogos salieron con una calidad fotográfica asombrosa; los colores eran vibrantes y los textos negros eran nítidos, reflejando el lujo de la marca sin desperdiciar ni un solo gramo de papel por errores técnicos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
