---
name: pagos-y-suscripciones-stripe-master-performance
description: "Pagos y Suscripciones (Stripe Master v2.0) es la competencia técnica de alto nivel para integrar, orquestar y escalar ecosistemas de cobro digital. No es solo \"poner un botón de pago\"; es Ingeniería de Ingresos Recurrentes. Úsala para tareas de Ventas y Comercio Electrónico: stripe-master, payments-infrastructure, saas-billing, subscription-management, fintech-ops, checkout-optimization."
title: Pagos y Suscripciones (Stripe Master Performance)
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-17
category: 06. Ventas y Comercio Electrónico
subcategory: Pagos y Suscripciones
tags: [stripe-master, payments-infrastructure, saas-billing, subscription-management, fintech-ops, checkout-optimization, webhooks, dunning-management, recursive-revenue, pci-compliance]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 585
---

## 0. Filosofía Human-Centric AI
*Esta habilidad democratiza el acceso a infraestructuras financieras de élite, utilizando la tecnología para automatizar la monetización ética y permitir que los creadores se centren en aportar valor mientras el sistema gestiona la entrada de recursos de forma segura y transparente.*

**El Rol del Humano:** El Arquitecto de Pagos debe ser un "Garante de la Integridad Financiera". La IA puede predecir qué suscripciones tienen riesgo de ser canceladas (Churn prediction), optimizar los reintentos de cobro de tarjetas fallidas (Smart Retries) y detectar patrones de fraude en milisegundos, pero solo el humano puede diseñar una política de precios justa que refleje el valor real aportado, gestionar devoluciones con empatía en casos de dificultad del cliente y asegurar que el modelo de negocio sea sostenible, ético y respetuoso con la privacidad de los datos financieros del usuario.
**Empoderamiento:** Usamos la tecnología para sustituir la burocracia bancaria por un motor de ingresos fluido que funciona las 24 horas, liberando al profesional para escalar su impacto.

---

## 1. Descripción Detallada
Pagos y Suscripciones (Stripe Master v2.0) es la competencia técnica de alto nivel para integrar, orquestar y escalar ecosistemas de cobro digital. No es solo "poner un botón de pago"; es **Ingeniería de Ingresos Recurrentes**. Se basa en el ecosistema **Stripe** para gestionar el ciclo de vida completo del dinero: desde el **Checkout Seguro** y la gestión de planes dinámicos, hasta la orquestación de **Webhooks** para recibir notificaciones sobre el estado de los pagos y suscripciones de forma asíncrona.

## 2. Escenarios de Aplicación
- **Modelos de Suscripción SaaS:** Gestión de niveles (Free, Pro, Enterprise), upgrades, downgrades y periodos de prueba.
- **Plataformas de E-commerce de Pago Único:** Procesamiento de transacciones seguras con cumplimiento PCI de nivel 1.
- **Marketplaces y Pagos Divididos (Connect):** Distribución automática de fondos entre múltiples vendedores y la plataforma.
- **Sistemas de Facturación B2B (Invoicing):** Automatización del envío de facturas legales y recordatorios de pago.
- **Monetización de Contenido (Paywalls):** Control de acceso en tiempo real basado en el estado de la suscripción del usuario.

## 3. Requisitos de Implementación
- **Stack Tecnológico Robusto:** Uso de Stripe SDK y herramientas de CLI para pruebas de integración local.
- **Arquitectura de Servidor Segura:** Manejo estricto de variables de entorno y validación de firmas de Webhook.
- **Cumplimiento Normativo (SCA/GDPR):** Implementación de autenticación reforzada y gestión de datos conforme a ley.

---

## 4. Diferencial: Cobro Manual vs. Stripe Master v2.0

| Dimensión | Enfoque Tradicional (Legacy) | Stripe Master (v2.0) |
| :--- | :--- | :--- |
| **Seguridad** | Manejo de datos sensibles (Riesgo). | Tokenización total (Seguridad PCI Máxima). |
| **Fricción** | Transferencias o formularios lentos. | Apple/Google Pay y 1-Click Checkout. |
| **Recurrencia** | Recordatorios manuales de pago. | Cobro automático y gestión de fallos. |
| **Escalado** | Proporcional a la administración. | Totalmente automatizado (1 a 1M clientes). |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Arquitectura de Productos y Flujo Transaccional
**Objetivo:** Crear un catálogo de precios que sea fácil de consumir y difícil de romper.
1.  **Definición de 'Price IDs':** IA ayuda a estructurar el catálogo (Ej: Mensual vs Anual con descuento) y sugiere el modelo de cobro (Flat fee, Metered, Tiered).
2.  **Seguridad en el Endpoint de Webhook:** Implementación de lógica de "Idempotencia" para no procesar dos veces el mismo pago.

**Prompt Maestro de Implementación de Pagos:**
```text
Actúa como un Senior Fintech Engineer y Experto en Arquitectura Stripe. Diseña el sistema de pagos para [NOMBRE_PROYECTO]. 
1. Estructura el Catálogo: Define 3 planes de suscripción y sus correspondientes metadatos para el CRM. 
2. Diseña el Flujo de 'Checkout': ¿Cómo integramos Stripe Checkout para que sea 'Seamless' y no parezca que el usuario sale de nuestra web? 
3. Lógica de 'Webhook': Redacta el pseudocódigo para manejar los eventos 'invoice.paid' y 'customer.subscription.deleted'. 
4. Plan de Gestión de Fallos (Dunning): ¿Qué pasa si la tarjeta falla? Define la secuencia de reintentos y correos de aviso. 
5. Configuración de 'Portal de Cliente': ¿Qué acciones permitimos que el usuario haga solo (Cerrar cuenta, Cambiar tarjeta, Descargar facturas)?
```

### Fase 2: Automatización, Reporting Financiero y SCA
... (Expansión técnica sobre el uso de 'Stripe Tax' para cálculo automático de IVA/VAT, la integración de pagos móviles biométricos y la creación de Dashboards de Revenue en tiempo real con métricas de MRR y Churn) ...

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
