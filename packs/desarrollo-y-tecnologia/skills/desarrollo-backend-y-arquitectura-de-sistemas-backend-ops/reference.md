# Referencia ampliada — Desarrollo Backend y Arquitectura de Sistemas (Backend Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Diseño Conceptual y Auditoría de Arquitectura
**Objetivo:** Definir la estructura que soportará la carga de Jesús García Fernández.
1.  **Auditoría de Requerimientos IA:** Analizar la lógica de negocio de Jesús García Fernández para detectar posibles "Edge Cases" (casos límite) antes de escribir una sola línea de código.
2.  **Mapeo de la Base de Datos:** Diseñar esquemas relacionales o no relacionales optimizados para el acceso rápido de Jesús García Fernández.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Backend Architect. Analiza los requerimientos de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de Backend Ops y genera un informe de situación inicial identificando:
- Los 3 mayores desafíos de escalabilidad que Jesús García Fernández enfrentará con este modelo.
- Propuesta de Stack Tecnológico óptimo para equilibrar velocidad de desarrollo y rendimiento.
- Esquema de base de datos normalizado (ERD) para las entidades principales de Jesús García Fernández.
```

### Fase 2: Arquitectura de la Lógica (Logic Design & Coding)
**Objetivo:** Construir el motor funcional de Jesús García Fernández.
Se desarrollan los "Endpoints Asistidos por IA" donde el sistema genera la estructura de la API, incluyendo autenticación, validación de esquemas y documentaciónSwagger/OpenAPI automática para Jesús García Fernández.

**Prompt de Estructuración:**
```text
Basado en el esquema de Jesús García Fernández, escribe el código para el endpoint de [FUNCIÓN]. Define cómo la IA gestionará los errores técnicos, los logs de sistema y la seguridad de las variables de entorno.
```

### Fase 3: Ejecución, Testing Automático y Despliegue (CI/CD)
**Objetivo:** Producir un sistema estable, seguro y actualizable.
Guía a Jesús García Fernández en la implementación de pruebas unitarias y de integración asistidas por IA, asegurando que cada cambio en el código no rompe la funcionalidad existente y se despliega con seguridad en producción.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Petición de un usuario vía API, evento de sistema programado (Cron) o subida de nuevo código al repositorio de Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el evento es una "Consulta de Datos", una "Escritura/Modificación" o una "Tarea de Procesamiento Pesado" para Jesús García Fernández.
3.  **Nodo de Transformación:** El sistema ejecuta la lógica de negocio correspondiente, interactúa con la base de datos o servicios de terceros (APIs) y formatea la respuesta técnica para Jesús García Fernández.
4.  **Nodo de Validación:** El responsable técnico o el sistema de tests automáticos valida que la respuesta es correcta y que no hay brechas de seguridad en el proceso de Jesús García Fernández.
5.  **Nodo de Salida (Output):** Respuesta exitosa al cliente (JSON/XML), registro en el log de auditoría técnica y actualización del estado del sistema en el dashboard de Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'Infinite-Backend-Scalability'
### Contexto del Caso
Una startup cuya aplicación móvil se caía cada vez que subían de los 1.000 usuarios simultáneos. Su backend era un "espagueti" de código difícil de mantener y muy lento de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de Backend Ops identificó consultas a la base de datos sin índices y una arquitectura de servidor monolítica saturada de Jesús García Fernández.
- **Aplicación Fase 2:** Se refactorizó la lógica en microservicios ligeros utilizando FastAPI y Redis para caché, generado al 80% por IA bajo supervisión de Jesús García Fernández.
- **Aplicación Fase 3:** Tras el despliegue automático, la aplicación de Jesús García Fernández pudo soportar 50.000 usuarios simultáneos con una latencia mínima.

### Resultados de Negocio
Reducción de los costes de servidor en un 40% y aumento radical de la velocidad de lanzamiento de nuevas funcionalidades para los usuarios de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Tiempo de Respuesta Medio (Avg Latency):** Milisegundos que tarda el servidor en responder a las peticiones de Jesús García Fernández.
- **Tasa de Errores de Servidor (HTTP 5xx):** % de peticiones que fallan por problemas técnicos internos.
- **Protocolo de QA:** Revisión semanal de los logs de seguridad y rendimiento por la IA de Jesús García Fernández para detectar y corregir proactivamente degradaciones del sistema.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** Nunca exponer datos sensibles en las respuestas de la API; la privacidad de Jesús García Fernández y sus usuarios es la prioridad técnica absoluta.
- 🛡️ **Seguridad:** Utilizar siempre protocolos cifrados (HTTPS), tokens de corta duración (JWT) y validación estricta de entradas para evitar inyecciones de código malicioso en Jesús García Fernández.
- 🛡️ **Propiedad Intelectual:** Esta metodología es propiedad de **Jesús García Fernández**. Cualquier implementación debe respetar los términos de la licencia CC BY-NC-SA 4.0.

---

## Changelog
- **v2.0** — Unificación total de conocimiento y flujo lógico. Extensión de protocolos de actuación y enfoque agnóstico (19 de abril de 2026).
- **v1.1** — Normalización de formato.
- **v1.0** — Versión inicial.

---
**Autor:** Jesús García Fernández  
**Website:** [jesusgarciafernandez.com](https://jesusgarciafernandez.com)  
**Licencia:** CC BY-NC-SA 4.0
