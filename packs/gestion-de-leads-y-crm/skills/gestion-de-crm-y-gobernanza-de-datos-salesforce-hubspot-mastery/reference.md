# Referencia ampliada — Gestión de CRM y Gobernanza de Datos (Salesforce & HubSpot Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de sincronización sistémica.*

1.  **Trigger:** Un cambio de estado en una plataforma externa (Ej: Pago completado en Stripe) o una acción manual en el CRM.
2.  **Nodo de Transformación de Datos:** El sistema traduce el input externo al formato del CRM (Mapeo de campos).
3.  **Nodo de Lógica de Negocio:** ¿Es un cliente nuevo o existente? El sistema actualiza el registro correspondiente y dispara las acciones de post-venta.
4.  **Nodo de Verificación de Integridad:** Se comprueba que no hay duplicados y que los campos obligatorios están rellenados antes del commit final.
5.  **Output:** CRM actualizado y "limpio"; notificaciones enviadas a administración y ventas para iniciar la fase de entrega del servicio.

---

## 7. Ejemplo Práctico: Empresa de Servicios de Limpieza Industrial
**Reto:** Perdían el 20% de las renovaciones de contratos anuales porque nadie se acordaba de llamar al cliente un mes antes del vencimiento.
**Acción v2.0:** Se configuró un workflow en el CRM que 45 días antes de la fecha de caducidad creaba un "Deal" de renovación, asignaba una tarea al comercial y enviaba un email automático de cortesía al cliente agendando una revisión técnica.
**Resultado:** La tasa de renovación subió al 98% en el primer año. El equipo administrativo ahorró 10 horas semanales que antes dedicaban a buscar fechas en archivos Excel antiguos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
