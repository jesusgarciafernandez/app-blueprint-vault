# Referencia ampliada — Uso Eficiente de Slack y Discord (Collaborative Ops Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Canales y Diseño del Manual de Estilo
**Objetivo:** Limpiar el ruido histórico y establecer las nuevas reglas de juego.
1.  **Purgado de Canales e Instalación de Nomenclatura:** IA ayuda a categorizar canales obsoletos y a renombrar los actuales con prefijos lógicos (Ej: `proj-`, `dept-`, `team-`).
2.  **Configuración del 'Dispatcher de Alertas':** Selección de qué notificaciones de herramientas externas merecen llegar al chat y a qué canal específico.

**Prompt Maestro de Diseño Colaborativo (Collab Architect):**
```text
Actúa como un Senior Productivity Engineer y Experto en Comunicación Organizacional. Diseña el entorno de [SLACK/DISCORD] para: [EQUIPO/PROYECTO]. 
1. Estructura de Canales Maestra: Propón una lista de 10 canales esenciales con sus prefijos y propósitos claros para evitar solapamientos. 
2. Guía de Notificaciones por Rango: Define qué configuración de avisos debe tener un perfil de [JUNIOR/SENIOR/MANAGER] para maximizar su tiempo de foco. 
3. Manual de Etiqueta 'Anti-Ruido': Redacta las 5 leyes sagradas del espacio (Ej: No saludar sin mensaje posterior, Hilos obligatorios, Uso de emojis como estado). 
4. Workflow de Integración Operativa: ¿Cómo conectaremos [HERRAMIENTA_EXTERNA] para que envíe resúmenes diarios en lugar de alertas cada minuto? 
5. Protocolo de 'Out of Office' Dinámico: Diseña cómo el equipo comunicará sus estados (En foco, En reunión, Comiendo) para gestionar las expectativas de respuesta.
```

### Fase 2: Ejecución, Entrenamiento del Equipo y Refactorización del Flujo
... (Expansión técnica sobre el uso de la técnica de 'Channel Canvas' para documentar el propósito de cada canal, la implementación de un proceso de 'Auditoría Mensual de Canales', y la monitorización de la 'Métrica de Salud de Hilos' para asegurar que la información no se pierde en conversaciones planas) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de centro de mando.*

1.  **Trigger:** Recepción de un mensaje en un canal, mención directa o cambio de estado de un usuario.
2.  **Nodo de Clasificación y Resumen Transversal:** El sistema analiza las conversaciones activas y genera un "Daily Summary" para los miembros que estaban en modo 'Deep Work'.
3.  **Nodo de Acción desde el Chat:** El sistema permite ejecutar tareas externas (Ej: "Crear ticket en Jira", "Aprobar factura") mediante comandos de texto o botones integrados en el chat.
4.  **Nodo de Limpieza y Archivo Automático:** La IA detecta canales que llevan inactivos >30 días y sugiere su archivo para mantener el espacio de trabajo ligero.
5.  **Output:** Espacio de trabajo zen y altamente productivo; reducción drástica de interrupciones; registro histórico impecable; equipo alineado y con foco.

---

## 7. Ejemplo Práctico: La Agencia 'CreativeFlow'
**Reto:** En 'CreativeFlow', los diseñadores se quejaban de que no podían terminar un diseño porque los clientes y directores les "asaltaban" por Slack constantemente. La información de los proyectos estaba dispersa en 5 canales diferentes y nadie sabía dónde estaba la última versión de los logos.
**Acción v2.0:** Implementaron Skill 284. Crearon canales únicos por cliente (`client-nom-proyecto`). Prohibieron los mensajes directos para temas técnicos (todo a hilos en canales públicos). Instalaron un bot que resúme los acuerdos tomados en cada hilo al terminar el día.
**Resultado:** Las interrupciones bajaron un 60%. Los diseñadores ahora activan el modo 'Deep Work' 4 horas al día sin miedo a perderse nada importante. La velocidad de entrega de los proyectos subió un 30% porque la información es fácil de encontrar y no hay que preguntar tres veces lo mismo.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
