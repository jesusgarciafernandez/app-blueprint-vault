# Referencia ampliada — Diseño y Testing Conversacional con N8N (Agentic Workflow Engineering)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de orquestación inteligente.*

1.  **Trigger:** Recepción de un evento desde un sistema externo o activación por tiempo (cron).
2.  **Nodo de Pre-procesamiento y Limpieza:** El sistema normaliza los datos de entrada para que sean digeribles por los nodos siguientes.
3.  **Nodo Agéntico de Decisión:** Un agente inteligente evalúa el contexto y decide qué rama del flujo ejecutar o qué herramienta externa invocar.
4.  **Nodo de Ejecución y Validación:** Se realizan las acciones (Ej: Guardar en DB, enviar Email) y se verifica que la respuesta sea correcta.
5.  **Output:** Acción completada; logs registrados; notificación de estado enviada al usuario o administrador; reporte de performance disponible.

---

## 7. Ejemplo Práctico: SaaS de Reclutamiento 'TalentBot'
**Reto:** 'TalentBot' recibía cientos de CVs por email y los reclutadores perdían horas leyéndolos para ver si cumplían los requisitos mínimos. El flujo manual era lento y propenso a errores.
**Acción v2.0:** Implementaron Skill 255. Crearon un workflow en N8N que escucha los emails, extrae el PDF, usa un agente de IA para analizar el CV contra la oferta de empleo y puntúa al candidato del 1 al 10.
**Resultado:** Los reclutadores ahora solo reciben los 3 mejores candidatos de cada posición con un resumen de sus puntos fuertes. El tiempo de filtrado inicial bajó de 48 horas a 2 minutos. El flujo fue probado en un Sandbox con 100 CVs falsos antes de ser activado para candidatos reales.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
