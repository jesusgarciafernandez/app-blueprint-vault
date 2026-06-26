# Referencia ampliada — Agentes de Voz e Inteligencia Telefónica (Voice AI Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Flujo Verbal y Selección de Identidad
**Objetivo:** Definir cómo debe sonar el agente y qué problemas va a resolver.
1.  **Diseño de la 'Persona' del Agente de Voz:** IA ayuda a elegir el género, tono, velocidad y calidez de la voz basándose en la imagen de la marca.
2.  **Mapeo del Grafo de Conversación Telefónica:** Definición de los caminos críticos (Happy Path) y las rutas de escape si el bot no entiende bien.

**Prompt Maestro de Arquitectura de Voz (Voice Architect):**
```text
Actúa como un Senior Conversational Designer y Voice AI Engineer. Diseña el agente telefónico para: [PROPÓSITO_LLAMADA]. 
1. Personalidad y Script Maestro: Redacta el saludo inicial y las 3 preguntas clave que aseguren una conversación fluida y orientada a [OBJETIVO]. 
2. Configuración de 'First-Sentence' y Latencia: Define cómo reaccionará el bot al descolgar para generar confianza inmediata (Ej: Pausa respiratoria natural). 
3. Definición de Herramientas Verbales (Tool-use): Describe qué acciones podrá disparar el bot en medio de la charla (Ej: crear_lead(), agendar_cita(fecha), enviar_sms_confirmacion()). 
4. Gestión de Interrupciones y Silencios: ¿Cómo debe actuar el bot si el humano le interrumpe a mitad de frase? Define los parámetros de agresividad/pasividad. 
5. Protocolo de 'Human Hand-off': ¿Bajo qué palabras clave o situaciones de frustración el bot debe transferir la llamada a un operador humano real?
```

### Fase 2: Ejecución, Pruebas de Latencia y Análisis de 'Call Transcripts'
... (Expansión técnica sobre el uso de la técnica de 'Prompt-Injection Monitoring' en voz, la implementación de un proceso de 'Auditoría de Conversión Telefónica', y la monitorización de la 'Métrica de Sentimiento Final' para asegurar que el usuario cuelga la llamada contento y con su problema resuelto) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de asistencia verbal.*

1.  **Trigger:** Entrada de una llamada telefónica al número virtual configurado o activación de una campaña outbound por el CRM.
2.  **Nodo de Inicialización de Sesión de Voz:** El sistema levanta el agente con su voz, personalidad e instrucciones específicas para esa llamada.
3.  **Nodo de Bucle Conversacional (STT -> LLM -> TTS):** La IA escucha, procesa la intención en milisegundos y genera la respuesta hablada de forma ininterrumpida.
4.  **Nodo de Ejecución de Tareas en Vivo:** El agente invoca herramientas externas (ej: mirar disponibilidad en calendar) durante la charla para dar respuestas reales.
5.  **Output:** Llamada finalizada con éxito; transcripción y resumen de la charla inyectados en el CRM; acciones programadas (ej: envío de contrato) ejecutadas.

---

## 7. Ejemplo Práctico: El Taller Mecánico 'QuickFix'
**Reto:** 'QuickFix' perdía 10 citas al día porque solo cogían el teléfono de 9 a 18. Los clientes llamaban para preguntar "¿Está mi coche?" y la recepcionista perdía 2 horas al día solo buscando estados de reparación.
**Acción v2.0:** Implementaron Skill 279. Un agente de voz atiende las 24h. Si un cliente pregunta por su coche, el bot le pide la matrícula, consulta el ERP y responde: "Sí, Juan, el cambio de aceite está listo. Puedes pasar a por él antes de las 20h".
**Resultado:** Cero llamadas perdidas. El 40% de las citas se agendan solas por teléfono fuera de horario. La recepcionista ahora solo gestiona la entrega física de llaves y cobros, mejorando la experiencia del cliente en el local.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
