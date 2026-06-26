# Referencia ampliada — Automatización Robótica de Procesos (RPA & Industrial Automation)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Procesos y Selección de Candidatos RPA
**Objetivo:** Elegir procesos con alto retorno de inversión (ROI) y baja complejidad de excepción.
1.  **Cálculo de Viabilidad (RPA Assessment):** IA ayuda a evaluar qué procesos son aptos basándose en el volumen de transacciones y la estabilidad de la interfaz.
2.  **Diseño del PDD (Process Definition Document):** Documentación paso a paso de la tarea humana actual antes de ser automatizada.

**Prompt Maestro de Arquitectura RPA (Bot Architect):**
```text
Actúa como un Senior RPA Solutions Architect y Experto en Excelencia Operativa. Diseña la solución robótica para el proceso: [NOMBRE_PROCESO]. 
1. Mapeo de Interacciones de UI: Describe la secuencia de clics, escritura y lecturas en las aplicaciones [APP_1] y [APP_2]. 
2. Estrategia de Selectores Robustos: ¿Cómo identificaremos el botón de 'Guardar' para que el bot no se pierda si la ventana cambia de tamaño o posición? 
3. Implementación de OCR Inteligente: Si el proceso incluye documentos PDF, define cómo extraeremos los campos [CAMPOS_DIGNÓSTICO] con alta confianza. 
4. Lógica de Gestión de Errores (Error Handler): Diseña el flujo de recuperación (Retry Scope) si la aplicación [APP_X] se congela o da un timeout. 
5. Protocolo de Escalado Humano: ¿Bajo qué condiciones específicas (BUSINESS EXCEPTIONS) el bot debe detenerse y enviar el caso a una persona para su revisión manual?
```

### Fase 2: Ejecución, Pruebas en Entorno de Usuario y Despliegue
... (Expansión técnica sobre el uso de la técnica de 'Headless Bots' para ahorrar recursos, la implementación de un proceso de 'Robot Queuing' para gestionar cargas de trabajo masivas, y la monitorización de la 'Tasa de Éxito de Transacciones' para optimizar la lógica del bot continuamente) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de fuerza digital.*

1.  **Trigger:** Disparo por tiempo, llegada de un nuevo archivo a una carpeta o una señal de un sistema externo.
2.  **Nodo de Inicialización de Robot:** El sistema arranca el bot, abre las aplicaciones necesarias y se loguea con credenciales seguras de tipo 'Robot Account'.
3.  **Nodo de Ejecución de Tarea (Core Logic):** El bot navega por la UI, realiza las acciones programadas (Extract/Write/Click) y gestiona los datos.
4.  **Nodo de Verificación de Resultado:** El sistema comprueba si el objetivo se cumplió (Ej: ¿Apareció el mensaje 'Guardado con éxito'?).
5.  **Output:** Proceso completado; reporte de transacciones generado; humano notificado si hubo excepciones; aplicaciones cerradas de forma limpia.

---

## 7. Ejemplo Práctico: Logística 'TransGlobal'
**Reto:** 'TransGlobal' tenía a 5 personas dedicadas exclusivamente a mirar las webs de 50 navieras diferentes para actualizar el estado de sus contenedores en su sistema interno de gestión (ERP de 1995 sin API). Los datos siempre tenían 24 horas de retraso.
**Acción v2.0:** Implementaron Skill 248. Desarrollaron un robot de RPA que se loguea en cada naviera cada hora, busca los contenedores activos, extrae la fecha de entrega y la escribe directamente en el ERP antiguo.
**Resultado:** Los 5 empleados ahora se dedican a la atención al cliente y ventas. El retraso de la información bajó de 24 horas a 30 minutos. El error humano en la transcripción de números de serie desapareció por completo.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
