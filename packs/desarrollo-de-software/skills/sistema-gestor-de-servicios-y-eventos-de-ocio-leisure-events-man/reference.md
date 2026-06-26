# Referencia ampliada — Sistema Gestor de Servicios y Eventos de Ocio (Leisure & Events Management System)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría Operativa y Diseño del Flujo de Venta
**Objetivo:** Crear un embudo de reserva sin fricciones que maximice la conversión.
1.  **Mapeo del Customer Journey:** IA ayuda a identificar y eliminar los pasos innecesarios en el proceso de reserva que causan abandono del carrito.
2.  **Definición de Tipos de Entrada e Inventario:** Diseño de la lógica de precios (Early bird, VIP, Descuentos) y límites de stock.

**Prompt Maestro de Diseño de Plataforma de Ocio (Event Architect):**
```text
Actúa como un Principal Product Manager y Experto en Leisure-Tech. Diseña el sistema gestor para el evento/servicio: [NOMBRE_EVENTO]. 
1. Arquitectura del Motor de Reservas: Define la lógica de disponibilidad (Ej: Por plazas, por tiempo, por recursos) y cómo manejaremos el 'Overbooking' preventivo. 
2. Flujo de Checkout de Alta Conversión: Describe las 3 fases del pago (Selección, Datos, Confirmación) asegurando una UX impecable y sin distracciones. 
3. Sistema de Ticketing y Acceso: Diseña el formato del ticket digital y el protocolo de validación rápida (Ej: App de escáner para staff con modo offline). 
4. Estrategia de Upselling y Cross-selling: Propón 2 servicios adicionales (Ej: Seguro de cancelación, merchandising) que se ofrezcan durante el proceso de compra. 
5. Panel de Control del Organizador (Dashboard): Define las 5 métricas clave que el organizador debe ver en tiempo real para tomar decisiones (Ej: ROI, Velocidad de venta, Segmentación de audiencia).
```

### Fase 2: Ejecución, Monitorización de Ventas y Logística
... (Expansión técnica sobre el uso de la técnica de 'Queuing Systems' para gestionar picos de tráfico en lanzamientos, la implementación de un proceso de 'Automated Reminders' para reducir los 'no-shows', y la monitorización de la 'Tasa de Fraude' para proteger los ingresos del evento) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de disfrute organizado.*

1.  **Trigger:** El usuario selecciona una fecha o actividad en la web y pulsa el botón de "Reservar Ahora".
2.  **Nodo de Verificación de Inventario:** El sistema bloquea temporalmente la plaza en milisegundos para evitar compras duplicadas.
3.  **Nodo de Procesamiento de Pago Seguro:** El sistema gestiona la transacción con la pasarela elegida y verifica el cargo correcto.
4.  **Nodo de Entrega de Credenciales:** Tras el éxito, se genera el ticket QR único y se envía por email junto con las instrucciones del evento.
5.  **Output:** Reserva confirmada; inventario actualizado; datos de venta reflejados en el panel del organizador y disparadores de recordatorio programados.

---

## 7. Ejemplo Práctico: Circuito de Karts 'SpeedZone'
**Reto:** 'SpeedZone' gestionaba las reservas por WhatsApp y papel. A menudo, dos grupos llegaban a la vez porque alguien olvidó apuntar una reserva, creando conflictos y devoluciones constantes. No sabían qué horas eran las más rentables.
**Acción v2.0:** Implementaron Skill 246. Desarrollaron un sistema de reserva web donde los usuarios eligen su tanda y pagan por adelantado. Instalaron una tablet en recepción para que el staff viera las próximas tandas.
**Resultado:** Los conflictos de reserva desaparecieron al 100%. Las ventas nocturnas subieron un 30% porque el sistema permitía reservar a las 2 AM cuando el staff no estaba. El dueño ahora sabe exactamente qué días necesita más personal basándose en los informes de venta del sistema.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
