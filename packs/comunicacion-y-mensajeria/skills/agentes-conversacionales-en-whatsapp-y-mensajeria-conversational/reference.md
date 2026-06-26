# Referencia ampliada — Agentes Conversacionales en WhatsApp y Mensajería (Conversational AI Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Casos de Uso y Diseño del Grafo Lógico
**Objetivo:** Definir qué va a hacer el agente y qué herramientas necesita.
1.  **Identificación de 'Puntos de Fricción' Conversacional:** IA ayuda a analizar los chats históricos para detectar las 10 preguntas que consumen el 80% del tiempo humano.
2.  **Mapeo de Integraciones Críticas:** Definición de qué APIs (Calendario, ERP, CRM) debe consultar el agente para ser útil de verdad.

**Prompt Maestro de Arquitectura de Agentes (Chat Architect):**
```text
Actúa como un Senior Conversational Designer y Lead AI Engineer. Diseña el agente de WhatsApp para: [NEGOCIO/PROPÓSITO]. 
1. Personalidad y Tono de Marca: Define el carácter del bot (Ej: Conciso, amable, experto) y las 3 reglas de oro de su estilo de redacción. 
2. Arquitectura RAG (Recuperación): ¿Qué documentos o base de datos le daremos para que aprenda sobre nuestro negocio? Define la estructura de los fragmentos de info. 
3. Definición de 'Tools' (Herramientas): Describe los 3 procesos externos que el bot podrá ejecutar (Ej: buscar_cita(fecha), consultar_precio(producto), escalar_a_humano()). 
4. Lógica de Manejo de Errores y Hallucinations: ¿Qué dirá el bot si no sabe la respuesta o si el sistema de IA falla? Diseña la salida elegante. 
5. Protocolo de Privacidad y Consentimiento: ¿Cómo pediremos el Opt-in y cómo manejaremos los datos sensibles compartidos en el chat?
```

### Fase 2: Ejecución, Pruebas de Estrés y Monitorización de Tasa de Resolución
... (Expansión técnica sobre el uso de la técnica de 'Few-Shot Prompting' para mejorar la precisión del agente, la implementación de un proceso de 'Supervisión Humana en Tiempo Real', y la monitorización de la 'Métrica de Resolución al Primer Intento' para validar la eficacia del sistema agéntico) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de asistencia inmediata.*

1.  **Trigger:** Recepción de un mensaje del usuario a través del webhook de la API de mensajería (WhatsApp/Telegram).
2.  **Nodo de Identificación y Contexto:** El sistema busca al usuario en la base de datos, recupera el historial de la charla y el historial de sus compras o preferencias.
3.  **Nodo de Procesamiento Agéntico (IA):** El agente procesa la intención, consulta la base de conocimientos RAG o invoca una herramienta externa (Tool) si es necesario.
4.  **Nodo de Ejecución y Respuesta:** El sistema lanza la acción (Ej: "Cita confirmada") y envía el mensaje de respuesta enriquecido al dispositivo del usuario.
5.  **Output:** Usuario con duda resuelta o tarea completada; logs de conversación guardados para entrenamiento; ahorro masivo de tiempo de soporte manual; lead calificado y listo.

---

## 7. Ejemplo Práctico: La Clínica 'DentalSmile'
**Reto:** 'DentalSmile' perdía el 30% de sus llamadas porque venían de noche o el equipo estaba ocupado. Muchos pacientes solo querían saber precios o pedir cita básica. La recepcionista pasaba 3 horas al día solo confirmando citas por teléfono.
**Acción v2.0:** Implementaron Skill 278. Integraron un agente en su WhatsApp Business que responde dudas técnicas de tratamientos usando RAG y está conectado al Google Calendar de los doctores.
**Resultado:** El 60% de las nuevas citas ahora se cierran solas por WhatsApp a cualquier hora. La recepcionista ahora solo gestiona los casos clínicos complejos y la atención física en la clínica. Las facturación ha subido un 20% gracias a la respuesta instantánea nocturna que antes se perdía.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
