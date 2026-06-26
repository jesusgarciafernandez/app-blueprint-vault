# Referencia ampliada — Big Data Engineering (Distributed Computing & Spark Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de procesamiento escalable.*

1.  **Trigger:** Llegada de archivos masivos al Data Lake o acumulación de eventos en una cola de mensajes (Kafka).
2.  **Nodo de Orquestación de Jobs:** El sistema levanta dinámicamente el clúster (Ej: Databricks Job) y lanza el pipeline de procesamiento.
3.  **Nodo de Procesamiento Distribuido:** Los nodos de computación ejecutan la lógica en paralelo sobre fracciones del total del dato.
4.  **Nodo de Validación y Consolidación de Resultados:** IA verifica que el procesamiento ha terminado satisfactoriamente y actualiza los metadatos del Data Lake.
5.  **Output:** Datos masivos procesados y disponibles; el sistema de BI es notificado para refrescar los informes de alto nivel.

---

## 7. Ejemplo Práctico: Multinacional 'GlobalShop'
**Reto:** Su sistema SQL tardaba 18 horas en calcular el cierre de ventas mundial diario de 10.000 tiendas. El reporte llegaba siempre un día tarde.
**Acción v2.0:** Migraron a un ecosistema Spark sobre Databricks. La IA optimizó el particionamiento de ventas por "Tienda-Día-Categoría".
**Resultado:** El tiempo de proceso bajó de 18 horas a 12 minutos. El equipo de dirección pudo ver el cierre de ventas global poco después de terminar el turno, permitiendo cambios estratégicos inmediatos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
