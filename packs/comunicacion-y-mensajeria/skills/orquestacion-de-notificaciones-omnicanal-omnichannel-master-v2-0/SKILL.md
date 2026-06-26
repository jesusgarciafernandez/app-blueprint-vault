---
name: orquestacion-de-notificaciones-omnicanal-omnichannel-master-v2-0
description: "La Orquestación de Notificaciones Omnicanal (v2.0) es la competencia de gestionar flujos de comunicación proactiva a través de múltiples canales (Push, Email, SMS, WhatsApp). No es solo \"enviar avisos\"; es Ingeniería del Dispatcher Inteligente. Úsala para tareas de Comunicación y Mensajería: notifications, push, email, sms, fcm, resend."
title: Orquestación de Notificaciones Omnicanal (Omnichannel Master v2.0)
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-18
category: 19. Comunicación y Mensajería
subcategory: Comunicación Multicanal
tags: [notifications, push, email, sms, fcm, resend, omnichannel, engagement, transactional-messaging, low-code, api-integration, operational-rhythm, attention-management]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 004
---

## 0. Filosofía Human-Centric AI
*Esta habilidad empodera la conexión humana al asegurar que la información crítica llegue a la persona a través del canal más adecuado, en el momento preciso y con la relevancia justa, utilizando la orquestación omnicanal para evitar la saturación digital y transformar las notificaciones de simples interrupciones en valiosas señales de progreso y seguridad, devolviendo al usuario el control sobre su atención.*

**El Rol del Humano:** El Arquitecto de la Comunicación Relevante debe ser un "Garantes de la Oportunidad y la Calma". La IA y los motores de despacho pueden automatizar el envío de miles de mensajes por Email, Push o SMS, seleccionar el canal con mayor probabilidad de apertura basándose en el historial del usuario y personalizar el contenido en milisegundos, pero solo el humano posee la sensibilidad para diseñar flujos de comunicación que no resulten invasivos, la ética para proteger la privacidad en cada envío y la empatía para entender cuándo el silencio es más valioso que un aviso.
**Empoderamiento:** Usamos la tecnología para sustituir el spam caótico por un pulso de comunicación inteligente, asertivo y centrado en el usuario.

---

## 1. Descripción Detallada
La Orquestación de Notificaciones Omnicanal (v2.0) es la competencia de gestionar flujos de comunicación proactiva a través de múltiples canales (Push, Email, SMS, WhatsApp). No es solo "enviar avisos"; es **Ingeniería del Dispatcher Inteligente**. El enfoque v2.0 se centra en la **Cascada de Entrega y Preferencia**: el diseño de sistemas que priorizan canales de bajo coste y alta inmersión (Push), escalando a canales de mayor persistencia (Email) o urgencia (SMS/WhatsApp) según la importancia del mensaje y el comportamiento de lectura del usuario. Abarca la gestión técnica de tokens FCM, plantillas dinámicas multicanal y la monitorización de entregabilidad para asegurar que el "pulso" del sistema sea siempre rastreable y efectivo.

## 2. Escenarios de Aplicación
- **Alertas de Seguridad en Tiempo Real:** Envío instantáneo de códigos MFA o avisos de inicio de sesión sospechoso vía Push y Email simultáneo.
- **Gestión de Ciclos de Vida del Cliente (CRM):** Automatización de correos de bienvenida, recordatorios de carritos abandonados y felicitaciones personalizadas.
- **Notificaciones de Estado de Procesos Batch:** Avisos al usuario cuando una tarea pesada (Ej: Generación de vídeo o informe) ha finalizado correctamente.
- **Sistemas de Recuperación y Reconquista:** Dispatch de ofertas especiales mediante Push enriquecido para usuarios inactivos en la App.
- **Flujos Transaccionales Críticos:** Confirmaciones de compra, facturas automáticas y estados de envío con trackeo integrado multicanal.

## 3. Requisitos de Implementación
- **Domino de Plataformas de Notificación Líderes:** Manejo experto de Firebase Cloud Messaging (FCM), Resend/SendGrid para Email y Twilio para SMS/WhatsApp.
- **Habilidad en Gestión de Suscripciones y Tokens:** Capacidad para almacenar, renovar y limpiar de forma segura los identificadores de dispositivos (VAPID/FCM Tokens).
- **Conocimiento de Plantillas Dinámicas Multicanal:** Uso de Handlebars, JSX o Liquid para generar contenidos que se adapten a la estética de cada canal.
- **Capacidad de Análisis de Entregabilidad:** Manejo de Webhooks para rastrear aperturas, clics y rebotes (Bounce Rate) en tiempo real.

---

## 4. Diferencial: Notificaciones Aisladas vs. Orquestación Omnicanal v2.0

| Dimensión | Enfoque Legacy (Silos) | Orquestación Omnicanal (v2.0) |
| :--- | :--- | :--- |
| **Canal** | Fijo y único por tarea. | Dinámico y en cascada según importancia. |
| **Personalización** | Estática; mismo mensaje para todos. | Adaptativa; contenido basado en contexto. |
| **Saturación** | Alta; se envía por todo a la vez. | Controlada por preferencias y urgencia. |
| **Visibilidad** | Pobre; no se sabe si se leyó. | Total; trackeo de CTR y Delivery en tiempo real. |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Canales y Diseño de la Lógica de Despacho
**Objetivo:** Establecer la infraestructura y las reglas de envío en cascada.
1.  **Configuración del 'Dispatcher Core':** IA ayuda a definir el mapeo entre tipos de eventos (Ej: 'Venta', 'Error', 'Promo') y sus canales prioritarios.
2.  **Validación de Salud de Dominio:** Implementación de registros SPF, DKIM y DMARC para asegurar que el Email no termine en la carpeta de Spam.

**Prompt Maestro de Orquestación Multicanal (Notification Architect):**
```text
Actúa como un Senior Product Manager y Experto en Engagement Digital. Diseña el ecosistema de notificaciones omnicanal para: [PRODUCTO/PROYECTO]. 
1. Mapeo de Matriz Urgencia/Canal: Define qué eventos se envían por Push, cuáles por Email y cuáles requieren SMS basándote en la importancia para el usuario. 
2. Diseño de Cascada de Entrega: Configura la lógica: "Si no abre el Push en [X] minutos, envía Email; si es crítico y no lee Email, intenta WhatsApp". 
3. Arquitectura de Tokens FCM: Define el flujo seguro para capturar el FCM_TOKEN del usuario, almacenarlo en [BASE_DE_DATOS] y renovarlo periódicamente. 
4. Guía de Plantillas Dinámicas: Propón una estructura de variables (Ej: {{user_name}}, {{action_url}}) que funcione de forma consistente en todos los canales. 
5. Protocolo de 'Quiet Hours' y Frecuencia: ¿Cómo evitaremos saturar al usuario? Define límites diarios de envío y franjas horarias de no-interrupción.
```

### Fase 2: Ejecución, Monitorización de CTR y Ajuste de Criterios
... (Expansión técnica sobre el uso de la técnica de 'Deep Linking' en notificaciones Push, la implementación de un proceso de 'A/B Testing de Asuntos' en Emails transaccionales, y la monitorización de la 'Tasa de Suscripción' para analizar si el sistema está resultando molesto o valioso para el usuario final) ...

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
