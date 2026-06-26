# Referencia ampliada — Gestión de Bases de Datos y Workflows (Airtable Discovery & Automation)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de orquestación de datos.*

1.  **Trigger:** Cambio de estado de un registro (Ej: Checkbox "Aprobar" marcado) o recepción de datos vía Formulario.
2.  **Nodo de Validación y Enriquecimiento:** El sistema verifica que los campos obligatorios estén llenos y calcula fórmulas necesarias (Ej: Fecha de vencimiento + 7 días).
3.  **Nodo de Acción Transversal:** Airtable dispara una acción nativa (Ej: Crear registro en otra tabla) y una externa vía Webhook.
4.  **Nodo de Notificación de Éxito:** Envío de mensaje automático (Slack/Email) con el resumen del registro procesado.
5.  **Output:** Sistema operativo actualizado 24/7; información veraz y accesible para todo el equipo sin intervención manual.

---

## 7. Ejemplo Práctico: Agencia de Marketing 'GrowthBoost'
**Reto:** Gestionaban los proyectos en un Excel compartido. Se perdían fechas de entrega, no sabían qué freelance estaba libre y las facturas se hacían a mano.
**Acción v2.0:** Migraron a Airtable. Automatizaron que al asignar un freelance, este reciba un email con el briefing. Al marcar "Terminado", se genera el PDF de la factura automáticamente.
**Resultado:** Ahorro de 10 horas semanales de gestión administrativa. El equipo tiene visibilidad total del calendario y las facturas se emiten sin errores al segundo de terminar el trabajo.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
