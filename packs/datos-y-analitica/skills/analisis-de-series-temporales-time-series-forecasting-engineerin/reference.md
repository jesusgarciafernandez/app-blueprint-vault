# Referencia ampliada — Análisis de Series Temporales (Time-Series & Forecasting Engineering)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de anticipación rítmica.*

1.  **Trigger:** Final de un ciclo temporal (Día/Semana/Mes) o actualización de la serie de datos transaccionales.
2.  **Nodo de Limpieza e Imputación Temporal:** El sistema detecta huecos en la serie y los rellena mediante interpolación basada en la tendencia local.
3.  **Nodo de Inferencia de Forecasting por IA:** El modelo procesa el histórico completo y genera la proyección para el próximo período.
4.  **Nodo de Alerta por Desviación de Tendencia:** Si el dato real se sale significativamente del intervalo de confianza del modelo, se dispara una alerta de "Cambio de Comportamiento".
5.  **Output:** Pronóstico actualizado en el Dashboard; equipo de finanzas o stock informado sobre las necesidades futuras proyectadas.

---

## 7. Ejemplo Práctico: Cadena de Restaurantes 'GoHealthy'
**Reto:** Tiraban el 15% de la comida fresca a la basura porque compraban lo mismo todos los días. No tenían en cuenta que los lunes se vendía un 40% menos que los viernes.
**Acción v2.0:** Implementaron un modelo Prophet con los datos de ventas diarios de 3 años. La IA aprendió los patrones semanales y los picos de las vacaciones.
**Resultado:** Reducción del desperdicio de comida al 5%. Los pedidos a proveedores se automatizaron basándose en la predicción de ventas personalizada para cada día de la semana.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
