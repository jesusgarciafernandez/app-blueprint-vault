# Referencia ampliada — Gestión de Correo e Inbox Zero (Email & Communication Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Flujo y Purgado de la Bandeja de Entrada
**Objetivo:** Eliminar el ruido histórico y establecer las barreras de entrada.
1.  **Limpieza por Lotes (The Great Archive):** IA ayuda a archivar masivamente todos los correos anteriores a una fecha determinada para liberar la mente del pasado.
2.  **Configuración de 'Filtros de Primera Barrera':** Automatización del archivo de notificaciones de herramientas (Jira, Slack, Ads) que no requieren respuesta humana.

**Prompt Maestro de Arquitectura de Correo (Inbox Architect):**
```text
Actúa como un Senior Productivity Coach y Experto en Comunicación Ejecutiva. Diseña el sistema de Inbox Zero para: [PERFIL/ROL]. 
1. Diseño de Filtros Automáticos: Propón 5 reglas de filtrado que desvíen el 40% del correo entrante (newsletters, compras, notificaciones) fuera del Inbox principal. 
2. Guía de Procesamiento de 5 Pasos: Define la lógica de decisión rápida para cada correo (Ej: Si <2min -> Responder; Si tarea -> Todoist). 
3. Configuración de Etiquetas/Carpetas Funcionales: Establece una estructura mínima de 3 carpetas (Ej: @Acción, @Espera, @Archivo) para evitar el desorden. 
4. Diccionario de Snippets/Plantillas: Identifica las 5 respuestas recurrentes y redacta las plantillas que ahorren el 80% del tiempo de escritura. 
5. Protocolo de Bloques de Tiempo: Diseña el horario diario de "ataque al correo" para que no interrumpa las horas de trabajo profundo.
```

### Fase 2: Ejecución, Mantenimiento del Cero y Sincronización de Tareas
... (Expansión técnica sobre el uso de la técnica de 'Snooze' (Posponer) con criterio, la implementación de un proceso de 'Unsubscribe' masivo semanal para mantener la higiene, y la monitorización de la 'Métrica de Respuesta de Valor' para asegurar que el tiempo en el correo genera impacto real) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de silencio operativo.*

1.  **Trigger:** Recepción de un nuevo correo en el servidor o inicio de un bloque programado de procesamiento.
2.  **Nodo de Pre-limpieza y Triaje por IA:** El sistema analiza el contenido, detecta la intención (pregunta, spam, tarea, recibo) y aplica la etiqueta o filtro correspondiente.
3.  **Nodo de Sugerencia de Respuesta:** Para correos de información sencilla, la IA prepara un borrador de respuesta basado en la base de conocimientos del usuario.
4.  **Nodo de Sincronización con el Ecosistema:** Los correos marcados como 'Acción' se convierten automáticamente en tareas con link directo al mensaje original en el gestor de tareas principal.
5.  **Output:** Inbox vacío; tareas prioritarias registradas; newsletters curadas para lectura en bloques de ocio; humano con mente despejada de ruido digital.

---

## 7. Ejemplo Práctico: El Analista de Marketing 'Ahogado'
**Reto:** Diego recibía 200 correos al día entre reportes automáticos, peticiones de clientes y correos internos. Pasaba 4 horas al día leyendo y re-leyendo correos, sintiendo que no podía avanzar en sus campañas. Su Inbox tenía 1.500 mensajes sin leer.
**Acción v2.0:** Implementó Skill 274. Archivó todo lo anterior a este mes. Configuró filtros para que los reportes PDF se guardaran directamente en Drive. Definió dos bloques de 45 minutos (10:00 y 16:00) para el correo.
**Resultado:** Diego ahora mantiene su Inbox por debajo de 10 mensajes cada día. Ha recuperado 2,5 horas de su jornada que ahora dedica a la optimización estratégica de campañas. Sus clientes reciben respuestas más rápidas y precisas gracias al uso de plantillas personalizadas para las dudas frecuentes.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
