# Referencia ampliada — A/B Testing Data Analysis (Experimentation & Statistical Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de procesamiento de experimentos.*

1.  **Trigger:** El usuario entra en la experiencia y el motor de asignación le entrega la Variante A o B.
2.  **Nodo de Tracking de Eventos:** El sistema registra las conversiones y métricas secundarias asociadas a la variante del usuario.
3.  **Nodo de Análisis Estadístico en Tiempo Real:** IA monitoriza el progreso y calcula la probabilidad de que una variante sea ganadora.
4.  **Nodo de Decisión Asistida:** El sistema avisa al equipo cuando se ha alcanzado la significancia estadística requerida.
5.  **Output:** Reporte técnico de éxito o fracaso del test; actualización automática del 100% del tráfico a la variante ganadora si el resultado es concluyente.

---

## 7. Ejemplo Práctico: SaaS de Facturación 'EfficientPay'
**Reto:** Su página de precios tenía un 15% de abandono. Querían probar si poner los testimonios "arriba o abajo" afectaba a la conversión.
**Acción v2.0:** Diseñaron un test con 20.000 usuarios. La IA detectó que no había significancia estadística global, pero al segmentar por "móvil", la Variante B (testimonios arriba) ganaba por un 10%.
**Resultado:** Implementaron el cambio solo para usuarios móviles. La conversión total subió un 4%. Sin el análisis profundo v2.0, habrían descartado una mejora ganadora por falta de datos globales.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
