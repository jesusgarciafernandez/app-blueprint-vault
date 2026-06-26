# Referencia ampliada — Análisis Digital & GA4 (Google Analytics 4 & Measurement Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de monitorización del usuario.*

1.  **Trigger:** Interacción del usuario en la web o App (Ej: El usuario visualiza una promoción).
2.  **Nodo de Captura y Filtrado por GTM:** El sistema intercepta el evento, le añade el contexto necesario (User-ID, parámetros de sesión) y lo envía a GA4.
3.  **Nodo de Procesamiento por IA de Google:** GA4 procesa el hit, lo atribuye a un canal y actualiza las métricas predictivas del perfil de usuario.
4.  **Nodo de Alerta por Anomalía de Tráfico:** Si el tráfico cae un 50% respecto al patrón histórico de esa hora, se dispara una alerta de "Posible Error de Servidor o Etiquetado".
5.  **Output:** Dashboards y exploraciones actualizadas en tiempo real; equipo de producto informado sobre el rendimiento de cada nueva funcionalidad lanzada.

---

## 7. Ejemplo Práctico: Portal de Viajes 'SkyBook'
**Reto:** No sabían por qué el 60% de los usuarios abandonaban en el paso de "pago". Sospechaban del precio, pero no tenían pruebas.
**Acción v2.0:** Implementaron GA4 con métricas de "Error de Formulario" personalizadas en GTM. La IA detectó que el 40% de los abandonos ocurrían por un error técnico al validar el código postal que el sistema no reportaba.
**Resultado:** Arreglaron el bug. La conversión subió un 12% en una semana. No fue el precio, fue la fricción detectada gracias a una analítica de eventos granular.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
