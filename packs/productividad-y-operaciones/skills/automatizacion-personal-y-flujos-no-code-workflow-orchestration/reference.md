# Referencia ampliada — Automatización Personal y Flujos No-Code (Workflow Orchestration)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Procesos y Diseño del Ecosistema
**Objetivo:** Identificar los cuellos de botella manuales y diseñar la solución técnica.
1.  **Inventario de Tareas Repetitivas:** IA ayuda a cuantificar el tiempo perdido en tareas mecánicas y prioriza qué flujo "duele" más.
2.  **Selección de la 'Gala' de Automatización:** Decidir qué herramienta es mejor para el caso (Ej: Zapier para rapidez, Make para multirutas).

**Prompt Maestro de Automatización Personal (Efficiency Architect):**
```text
Actúa como un Senior Automation Consultant y Experto en Productividad No-Code. Diseña el ecosistema de automatización para el proceso: [DESCRIPCIÓN_PROCESO]. 
1. Mapeo de Flujo de Datos: Identifica la 'App A' (Trigger), los pasos de transformación intermedios (Filtros/Parseo de texto) y la 'App B' (Action final). 
2. Diseño de Lógica Condicional: Si [CONDICIÓN_X], el flujo debe hacer 'Y'; si no, debe hacer 'Z'. Redacta la lógica detallada para el Router. 
3. Configuración de Webhooks y API: Define las cabeceras y los datos del JSON que necesitamos enviar para que la integración sea segura y completa. 
4. Plan de Gestión de Errores: ¿Qué sucede si una de las apps falla? Diseña un nodo de notificación de error que avise al humano si el flujo se detiene. 
5. Auditoría de Seguridad: Verifica que los datos sensibles (Ej: PII) se transfieran de forma cifrada y solo entre las herramientas autorizadas.
```

### Fase 2: Ejecución, Pruebas en Sandbox y Despliegue Silencioso
... (Expansión técnica sobre el uso de la técnica de 'Iterators' para procesar listas de datos de una sola vez, la implementación de un proceso de 'Cleanup' mensual para eliminar flujos obsoletos que consumen recursos, y la monitorización de las 'Tasks' mensuales para optimizar los costes de las suscripciones de automatización) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de fluidez operativa.*

1.  **Trigger:** Ocurre un evento en una aplicación (Ej: Nuevo pago, llegada de email, creación de fila en Excel).
2.  **Nodo de Validación y Filtro:** El sistema comprueba si el evento cumple los criterios deseados antes de continuar (Ej: Solo emails con asunto 'URGENTE').
3.  **Nodo de Transformación de Datos:** Se limpia el texto, se formatean fechas o se realizan cálculos necesarios para la siguiente aplicación.
4.  **Nodo de Acción Multicanal:** La información se distribuye a una o varias herramientas de forma paralela (Ej: Crear factura Y notificar en Slack).
5.  **Output:** Tarea completada sin intervención humana; reporte de ejecución disponible en el historial de la automatización; humano notificado solo si se requiere su atención.

---

## 7. Ejemplo Práctico: Consultoría 'AgileGrowth'
**Reto:** 'AgileGrowth' perdía 10 horas semanales copiando datos de clientes desde su web a un Excel, creando a mano las carpetas en Drive y enviando correos de bienvenida personalizados. A veces tardaban 2 días en responder a un nuevo lead.
**Acción v2.0:** Implementaron Skill 247. Crearon un flujo en Make que, al recibir un lead, lo guarda en el CRM, crea automáticamente la carpeta del proyecto en Drive, genera el contrato con sus datos y envía el email de bienvenida al instante.
**Resultado:** El tiempo de respuesta bajó de 48 horas a 30 segundos. El equipo recuperó 40 horas mensuales que ahora dedican a dar un servicio premium a esos mismos clientes, eliminando por completo el error de "carpeta mal nombrada" o "email olvidado".

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
