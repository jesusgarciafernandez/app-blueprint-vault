# Referencia ampliada — Python para Ciencia de Datos (Scientific Computing & Data Wrangling Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de procesamiento de datos por código.*

1.  **Trigger:** Recepción de un nuevo conjunto de datos crudos (Ej: Log de ventas del mes) en el servidor de analítica.
2.  **Nodo de Ejecución de Pipeline Python:** El sistema lanza automáticamente el script de limpieza predefinido.
3.  **Nodo de Validación y QA de Datos:** IA verifica que el dataset final cumple con los estándares de calidad esperados (no hay duplicados inesperados, los rangos son coherentes).
4.  **Nodo de Generación de Visualizaciones:** El sistema crea un set de gráficos .png o .html y los adjunta a un reporte.
5.  **Output:** Datos listos para el consumo; informe técnico y dashboard actualizado enviados a los responsables de área en minutos.

---

## 7. Ejemplo Práctico: Fintech 'SmartLend'
**Reto:** Tardaban 1 semana en limpiar los datos de las solicitudes de crédito que venían de 5 fuentes diferentes antes de poder evaluarlas.
**Acción v2.0:** Implementaron un pipeline en Python con Pandas. La IA automatizó el mapeo de columnas y la limpieza de duplicados entre fuentes.
**Resultado:** El tiempo de preparación de datos bajó de 40 horas a 2 minutos. Pudieron empezar a dar respuestas a los créditos en 24 horas en lugar de 10 días.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
