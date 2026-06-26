# Referencia ampliada — LLM Orchestration (LangChain & Modular AI Systems)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de integración inteligente.*

1.  **Trigger:** Entrada del usuario o evento de sistema que requiere un razonamiento multi-paso.
2.  **Nodo de Planificación de Acción:** El orquestador analiza la meta y selecciona la primera herramienta o prompt de la secuencia.
3.  **Nodo de Ejecución de Tool/Chain:** La IA ejecuta la tarea, consulta la base de datos o API externa y recupera el resultado.
4.  **Nodo de Evaluación de Resultado:** El sistema verifica si la información obtenida es suficiente o si requiere iterar un paso más.
5.  **Output:** Resultado final consolidado y acción de software ejecutada (ej: email enviado); log de ejecución guardado para mejora continua.

---

## 7. Ejemplo Práctico: Agencia Inmobiliaria 'GeoMatch'
**Reto:** Los agentes perdían horas buscando propiedades compatibles con los deseos de los clientes y luego redactando emails personalizados.
**Acción v2.0:** Implementaron Orquestación LLM (Skill 220). Una cadena personalizada busca en la base de datos SQL del portal, recupera las fotos, usa un modelo de visión para describirlas y luego otro modelo redacta el email final según el perfil del cliente en el CRM.
**Resultado:** El proceso pasó de 45 minutos a 15 segundos. La inmobiliaria ahora puede responder de forma personalizada al 100% de sus solicitudes en tiempo real, aumentando las visitas a propiedades un 40%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
