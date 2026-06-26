# Referencia ampliada — Limpieza de Datos & Wrangling (Data Integrity & Quality Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de purificación continua.*

1.  **Trigger:** Ingesta de nuevos datos crudos desde una fuente externa (API, CSV, DB).
2.  **Nodo de Perfilado Automático:** El sistema analiza la calidad inicial y detecta si el dataset está por debajo del umbral de limpieza aceptable.
3.  **Nodo de Transformación por Código:** IA ejecuta el pipeline de limpieza predefinido (Deduplicación -> Formateo -> Imputación).
4.  **Nodo de Validación Final:** Un proceso de QA verifica que las reglas de sanidad se cumplen (Ej: No hay precios negativos).
5.  **Output:** Datos íntegros volcados al Data Warehouse; notificación al equipo de analítica de que los nuevos datos están listos y limpios.

---

## 7. Ejemplo Práctico: Retailer 'ShopGlobal'
**Reto:** Tenían 50.000 clientes duplicados porque unos se registraban como "J. Perez", otros como "Juan Perez" y otros con el email en mayúsculas.
**Acción v2.0:** Aplicaron un pipeline de Data Wrangling con limpieza de texto y Fuzzy Matching. La IA detectó que el 30% de sus "clientes" eran en realidad las mismas personas con diferentes registros.
**Resultado:** Unificaron la base de datos de clientes. Ahorraron miles de euros en envíos de marketing duplicados y pudieron por primera vez calcular el Life Time Value (LTV) real de sus usuarios.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
