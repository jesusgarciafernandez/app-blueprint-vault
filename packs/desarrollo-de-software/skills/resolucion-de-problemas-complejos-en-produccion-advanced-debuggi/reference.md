# Referencia ampliada — Resolución de Problemas Complejos en Producción (Advanced Debugging & SRE)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Triaje, Contención y Recolección de Evidencias
**Objetivo:** Estabilizar el sistema y salvar los datos del incidente.
1.  **Activación de Protocolo de Alerta:** IA detecta la anomalía en las 'Golden Signals' (Error Rate > 5%) y notifica al responsable de guardia.
2.  **Aislamiento del Síntoma:** Evaluación de si el fallo es global o afecta solo a un subconjunto de usuarios o regiones.

**Prompt Maestro de Debugging Avanzado (Incident Commander):**
```text
Actúa como un Senior SRE (Site Reliability Engineer) y Experto en Troubleshooting de Sistemas Distribuidos. Diagnostica el incidente reportado en: [DESCRIPCIÓN_SÍNTOMA]. 
1. Análisis de Correlación: Revisa las métricas de CPU, Memoria y Error Rate en los últimos 30 minutos. ¿Qué cambió justo antes del fallo? (Ej: Un despliegue, un pico de tráfico). 
2. Búsqueda de Causa Raíz (RCA): Identifica los 3 tipos de logs más relevantes y propón la consulta exacta para encontrar el error común (Ej: 500 Internal Server Error en el servicio Auth). 
3. Hipótesis Operativas: Plantea 2 posibles causas (Ej: Agotamiento de conexiones a BD, Timeout de API de terceros) y describe cómo verificar cada una sin tumbar el sistema. 
4. Plan de Contención Inmediata: ¿Qué acción podemos tomar YA para mitigar el impacto? (Ej: Rollback de la última versión, aumentar nodos de cómputo, activar 'Circruit Breaker'). 
5. Protocolo de Comunicación: Redacta un mensaje transparente para los usuarios y stakeholders sobre el estado actual del incidente y el tiempo estimado de resolución.
```

### Fase 2: Resolución, Verificación y Aprendizaje (Post-mortem)
... (Expansión técnica sobre el uso de la técnica de 'Log Correlation' para seguir una petición a través de múltiples microservicios, la implementación de un proceso de 'Error Budgeting' para decidir cuándo priorizar la estabilidad sobre la velocidad de desarrollo, y la monitorización de las 'Custom Metrics' de negocio para asegurar que la funcionalidad se ha restaurado correctamente tras el parche) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de sanación sistémica.*

1.  **Trigger:** Superación de un umbral crítico de errores o latencia detectado por el sistema de monitorización.
2.  **Nodo de Pre-Diagnóstico con IA:** El sistema correlaciona el fallo con los últimos commits de código y cambios de configuración de infraestructura.
3.  **Nodo de Recolección de Contexto (Incident Snapshot):** Se capturan los últimos 5 minutos de trazas y logs detallados del area afectada para análisis posterior.
4.  **Nodo de Acción Sugerida o Automática:** El sistema sugiere un 'Rollback' automático si el fallo coincide con un deploy reciente, o escala recursos si es un problema de saturación.
5.  **Output:** Sistema estabilizado; informe preliminar de incidente generado automáticamente; sesión de Post-mortem agendada para mejora continua.

---

## 7. Ejemplo Práctico: Fintech 'SafePay'
**Reto:** 'SafePay' empezó a rechazar el 20% de los pagos aleatoriamente durante la hora de la comida. No había errores claros en el backend y el problema desaparecía solo al cabo de una hora.
**Acción v2.0:** Implementaron Skill 241 de Debugging Avanzado. Usaron trazado distribuido y descubrieron que un microservicio de 'Geolocalización' externo estaba tardando 2 segundos más de lo normal, causando que el Gateway de pagos cortase la conexión por timeout.
**Resultado:** Implementaron un 'Circuit Breaker' (Skill 231) para que, si el servicio externo fallaba o tardaba demasiado, se usara una ubicación por defecto o se saltase el check. El MTTR bajó de 60 minutos a 0 minutos, ya que el sistema ahora se auto-sana ante ese fallo específico.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
