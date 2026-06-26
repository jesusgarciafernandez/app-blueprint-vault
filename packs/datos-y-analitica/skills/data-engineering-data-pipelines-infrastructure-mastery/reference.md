# Referencia ampliada — Data Engineering (Data Pipelines & Infrastructure Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de tubería de información.*

1.  **Trigger:** Evento temporal (cron) o llegada de nuevos archivos al sistema de almacenamiento primario.
2.  **Nodo de Extracción (Ingestion):** El sistema lanza un worker de Python que se conecta a las fuentes origen y vuelca los datos en la capa Bronze.
3.  **Nodo de Transformación y QA:** IA revisa el esquema y ejecuta los scripts de limpieza, moviendo los datos validados a la capa Silver.
4.  **Nodo de Agregación de Negocio:** El motor de base de datos ejecuta las vistas Gold que unen tablas y calculan KPIs finales.
5.  **Output:** Tablas Gold listas para el BI; el sistema de orquestación marca el ciclo como "Exitoso" y libera recursos.

---

## 7. Ejemplo Práctico: E-commerce 'FashionFlow'
**Reto:** Tenían los datos de stock en Excel, los de ventas en Shopify y los de marketing en Facebook. Saber el beneficio real de un producto les llevaba 3 días de trabajo manual.
**Action v2.0:** Los ingenieros crearon un pipeline que une las 3 fuentes cada hora en un Data Warehouse en la nube.
**Resultado:** Ahora el equipo de compras sabe el beneficio exacto por SKU en tiempo real. Redujeron el stock inmovilizado un 20% al ver qué productos no tenían rotación rentable inmediatamente.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
