# Referencia ampliada — Comunicación Asíncrona y Documentación Eficaz (Asynchronous Flow Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Canales y Diseño de la Política Asíncrona
**Objetivo:** Establecer las reglas de juego y las herramientas del equipo.
1.  **Definición de 'Canales de Urgencia' vs 'Canales de Flujo':** IA ayuda a catalogar qué tipos de información van por dónde y qué niveles de respuesta se esperan.
2.  **Creación de Templates de 'Async-Post':** Estándares para el equipo sobre cómo redactar actualizaciones de proyecto o peticiones de ayuda.

**Prompt Maestro de Arquitectura Asíncrona (Async Architect):**
```text
Actúa como un Senior Operations Manager y Experto en Cultura de Trabajo Remoto. Diseña el manual de comunicación asíncrona para: [EQUIPO/PROYECTO]. 
1. Estructura del 'Mensaje Perfecto': Define los campos obligatorios (Ej: Contexto, ¿Hay bloqueo?, Acción requerida, Deadline sugerido) para peticiones en [SLACK/NOTION]. 
2. Política de Notificaciones y SLA: Define los tiempos de respuesta esperados según el canal y cómo los protegeremos (Ej: 'Modo No Molestar' obligatorio de 9 a 12). 
3. Caso de Escalado Síncrono: ¿Bajo qué circunstancias específicas DEBEMOS llamar o reunirnos? (Ej: Bloqueo de >2 horas, Conflicto emocional, Decisión irreversible). 
4. Uso de Video Asíncrono (Loom): Redacta una guía rápida sobre cuándo grabar la pantalla en lugar de escribir un documento de 10 páginas. 
5. Ritual de 'Daily Asíncrona': ¿Cómo sustituiremos la reunión matinal de 15 min por un sistema de reporte escrito que no interrumpa al equipo?
```

### Fase 2: Ejecución, Evangelización de la Calidad y Refactorización de Reuniones
... (Expansión técnica sobre el uso de la técnica de 'Public by Default' (Público por defecto) para maximizar la transparencia, la implementación de un proceso de 'Auditoría de Reuniones Semanal', y la monitorización de la 'Métrica de Disponibilidad de Deep Work' para asegurar que el equipo gana horas de foco real semanalmente) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de flujo persistente.*

1.  **Trigger:** Redacción de un nuevo mensaje en un canal de comunicación o detección de una duración excesiva de una reunión síncrona.
2.  **Nodo de Pre-limpieza y Estructuración:** El sistema analiza el texto del humano y sugiere añadir el contexto faltante antes de enviarlo (Ej: "¿Has incluido un pantallazo del error?").
3.  **Nodo de Resumen y Threading:** La IA agrupa mensajes relacionados en hilos temáticos y genera resúmenes diarios para que nadie tenga que leer 500 mensajes de chat.
4.  **Nodo de Transcripción y Documentación:** Las videollamadas inevitables se transcriben y sus puntos clave se inyectan automáticamente en la base de conocimientos (Notion/Wiki).
5.  **Output:** Comunicación fluida sin interrupciones; base de conocimientos actualizada orgánicamente; equipo con más tiempo de foco; cultura de transparencia total.

---

## 7. Ejemplo Práctico: La Consultora 'GlobalDesign'
**Reto:** 'GlobalDesign' tenía empleados en Madrid, Buenos Aires y Sídney. Siempre había alguien despierto trabajando pero perdían días enteros esperando respuestas de compañeros en otras zonas horarias. Las mañanas eran un caos de reuniones de "ponerse al día".
**Acción v2.0:** Implementaron Skill 281. Prohibieron las reuniones de estatus. Todo se comunica por hilos de Slack con un formato estricto: Contexto | Bloqueos | Acción. Usan Loom para explicar feedback de diseño.
**Resultado:** La velocidad de los proyectos se duplicó. Cada profesional trabaja en sus horas de máxima energía sin ser molestado. Al llegar a su escritorio, cada uno tiene en su 'Inbox' toda la información necesaria para avanzar el día entero sin depender de nadie más. La cultura de la empresa pasó de la "ansiedad de respuesta" a la "excelencia de entrega".

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
