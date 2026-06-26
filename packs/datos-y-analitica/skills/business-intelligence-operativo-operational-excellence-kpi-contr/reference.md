# Referencia ampliada — Business Intelligence Operativo (Operational Excellence & KPI Control)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control operativo continuo.*

1.  **Trigger:** Actualización regular del ERP o recepción de nuevos eventos desde un sensor o App móvil de operarios.
2.  **Nodo de Ingesta y Transformación (ELT):** El sistema vuelca los datos al Data Warehouse y calcula los agregados necesarios para el dashboard.
3.  **Nodo de Evaluación de Reglas de Negocio:** IA analiza los nuevos valores y los compara con los objetivos del día y las medias históricas.
4.  **Nodo de Acción Automática:** Si se detecta una desviación crítica, el sistema dispara flujos secundarios (Ej: Reasignación de tickets, aviso al responsable de mantenimiento).
5.  **Output:** Cuadros de mando actualizados en las pantallas de la organización; equipo proactivo y alineado con los objetivos del momento.

---

## 7. Ejemplo Práctico: Centro Logístico 'LogiSpeed'
**Reto:** No sabían por qué el 10% de los envíos salían tarde, provocando reclamaciones masivas. Echaban la culpa a "la falta de personal".
**Acción v2.0:** Implementaron un dashboard de BI Operativo. La IA visualizó el proceso completo y detectó que el cuello de botella estaba en la impresora de etiquetas, que fallaba a media mañana y retrasaba todo el empaquetado.
**Resultado:** Compraron una impresora mejor. La puntualidad subió al 99% sin contratar a nadie más. La eficiencia se logró gracias a la visibilidad del dato, no al aumento de recursos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
