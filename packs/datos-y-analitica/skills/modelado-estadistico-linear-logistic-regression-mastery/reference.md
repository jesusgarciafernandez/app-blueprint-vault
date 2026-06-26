# Referencia ampliada — Modelado Estadístico (Linear & Logistic Regression Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de inferencia continua.*

1.  **Trigger:** Finalización de un experimento de ventas o recepción de nuevos datos trimestrales de mercado.
2.  **Nodo de Limpieza y Ajuste:** El sistema preprocesa los datos y entrena el modelo lineal/logístico de forma automática.
3.  **Nodo de Control de Calidad Estadístico:** IA verifica que los p-values de las variables críticas siguen siendo significativos (< 0.05).
4.  **Nodo de Generación de Inferencia:** El sistema traduce los nuevos coeficientes a una breve nota de voz o texto explicativo (Ej: "La sensibilidad al precio ha subido un 5% este mes").
5.  **Output:** Modelo actualizado en producción; equipo de dirección informado automáticamente sobre el cambio en las palancas clave del negocio con base estadística sólida.

---

## 7. Ejemplo Práctico: Inmobiliaria 'UrbanMetrics'
**Reto:** Tasaban casas a ojo basándose en "lo que pedía el vecino". Fallaban en el 30% de las ventas por precio fuera de mercado.
**Acción v2.0:** Crearon un modelo de regresión múltiple con 2.000 operaciones históricas. La IA identificó que "la distancia al metro" en esa zona influía 3 veces más que "tener terraza".
**Resultado:** Los precios de tasación se alinearon con la realidad del mercado al 95%. El tiempo medio de venta bajó de 6 meses a 45 días al eliminar el sesgo emocional de los tasadores.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
