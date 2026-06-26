# Referencia ampliada — App Companion Educativo y de Seguimiento (Educational Mentor App)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Necesidades Formativas y Diseño del Flujo
**Objetivo:** Identificar los puntos clave de contacto entre mentor y aprendiz.
1.  **Mapeo de la 'Ruta del Alumno':** IA ayuda a identificar en qué momentos del proceso educativo el usuario suele perder motivación o necesitar más apoyo.
2.  **Definición de Métricas de Seguimiento:** Selección de los KPIs (Key Performance Indicators) que la app debe recolectar (Ej: Tiempo de estudio, tasa de acierto, estados de ánimo).

**Prompt Maestro de Diseño de App Companion (Mentor Architect):**
```text
Actúa como un Senior Product Manager y Experto en Psicología del Aprendizaje (EdTech). Diseña la App Companion para el programa: [NOMBRE_PROGRAMA]. 
1. Estructura de Secciones: Define las 3 pantallas principales (Ej: Mi Progreso, Centro de Recursos, Canal Directo) y su propósito funcional y educativo. 
2. Sistema de Notificaciones Inteligentes: Diseña 3 disparadores (Triggers) de notificaciones (Ej: Recordatorio de hábito fallido, Celebración de hito, Sugerencia de contenido nuevo). 
3. Flujo de Recolección de Feedback: Redacta el diseño de un formulario 'Micro-Checkin' semanal que tarde menos de 1 minuto en completarse pero dé datos valiosos al mentor. 
4. Gamificación y Logros: Propón un sistema de medallas o hitos que incentive la progresión constante y el sentido de logro del usuario. 
5. Protocolo de Intervención del Mentor: Define bajo qué condiciones (Ej: Alerta de inactividad de 5 días) el sistema debe pedir al mentor humano una intervención directa.
```

### Fase 2: Ejecución, Lanzamiento y Evolución del Contenido
... (Expansión técnica sobre el uso de la técnica de 'Push-to-Learn' para enviar pequeñas píldoras de conocimiento, la implementación de un proceso de 'A/B Testing de Mensajes' para optimizar la tasa de apertura de las notificaciones, y la monitorización de la 'Tasa de Abandono' (Churn Rate) del proceso educativo para ajustar el acompañamiento dinámicamente) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de crecimiento guiado.*

1.  **Trigger:** El usuario completa una actividad, registra un dato o se cumple un plazo de tiempo definido en el programa.
2.  **Nodo de Procesamiento de Progreso:** El sistema analiza el nuevo dato contra el plan de estudio y los objetivos personales del usuario.
3.  **Nodo de Respuesta Adaptativa:** El sistema lanza una notificación de refuerzo, desbloquea nuevo contenido o actualiza el gráfico de progreso visual.
4.  **Nodo de Alerta al Mentor:** Si se detectan anomalías o éxitos extraordinarios, se notifica al mentor para que realice una acción humana personalizada.
5.  **Output:** Usuario motivado y guiado; historial de aprendizaje enriquecido; reporte estratégico de salud del programa formativo disponible para el mentor.

---

## 7. Ejemplo Práctico: Programa de Mentoría 'LíderesPro'
**Reto:** 'LíderesPro' tenía una tasa de finalización de solo el 20% en su programa de 6 meses porque los participantes se sentían solos entre las sesiones Zoom mensuales y olvidaban aplicar lo aprendido.
**Acción v2.0:** Implementaron Skill 243. Crearon una App Companion simple donde los líderes registraban una "Acción Heroica" diaria y recibían una pregunta de reflexión corta cada mañana.
**Resultado:** La tasa de finalización subió al 85%. Los participantes reportaron sentir que el mentor estaba "con ellos en el bolsillo", y las sesiones mensuales fueron mucho más productivas porque el mentor ya conocía los retos reales superados durante el mes a través de los datos de la app.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
