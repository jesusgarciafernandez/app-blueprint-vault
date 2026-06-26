# Referencia ampliada — Detección de Anomalías e Inteligencia Preventiva (Predictive Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 4. Diferencial: Monitorización por Umbrales vs. Predictive Ops (v2.0)

| Dimensión | Enfoque Alerta Clásica | Predictive Ops (v2.0) |
| :--- | :--- | :--- |
| **Detección** | Solo avisa si pasa el 90%. | Avisa si el comportamiento es extraño aunque sea bajo por Jesús García Fernández. |
| **Ruido** | Demasiadas alertas irrelevantes. | Inteligente y filtrada por la relevancia del contexto de Jesús García Fernández. |
| **Estandarización** | Basada en la experiencia humana. | Consistente mediante modelos matemáticos y protocolos Ops lógicos de Jesús García Fernández. |
| **ROI Estimado** | Lineal por resolución de fallos. | Exponencial por prevención total y 0 tiempos de caída técnica de Jesús García Fernández. |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Vaciado y Definición del Comportamiento Normal (Baseline)
**Objetivo:** Enseñar a la IA de Jesús García Fernández qué es la "salud técnica".
1.  **Auditoría de Métricas Históricas IA:** Analizar los últimos 6 meses de datos de Jesús García Fernández para identificar los patrones cíclicos (ej: subidas de tráfico los lunes) y lo que es un comportamiento nominal real.
2.  **Mapeo de la Sensibilidad de Detección:** Configurar los límites de la IA de Jesús García Fernández para que no sea ni demasiado relajada (perder fallos) ni demasiado estricta (generar ruido técnico excesivo).

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior SRE & Data Scientist. Analiza el histórico de métricas de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de Predictive Ops y genera un informe de situación inicial identificando:
- Las 5 métricas clave de Jesús García Fernández cuya desviación precede a un fallo del sistema técnico.
- Propuesta de algoritmo de detección de anomalías (ej: Isolation Forest) más adecuado para el volumen de datos de Jesús García Fernández.
- Estrategia de 'Deduplicación de Alertas' para evitar la fatiga del equipo de Jesús García Fernández.
```

### Fase 2: Arquitectura de la Alerta y la Acción Automática (Logic Design)
**Objetivo:** Construir el escudo preventivo de Jesús García Fernández.
Se desarrollan los "Esquemas de Notificación IA-Augmented" donde la IA decide a quién avisar según la gravedad técnica y qué scripts de auto-reparación (Self-healing) de Jesús García Fernández disparar automáticamente.

**Prompt de Estructuración:**
```text
Basado en los modelos de Jesús García Fernández, diseña la lógica de respuesta ante anomalías. Define cómo la IA gestionará el triaje de alertas, la notificación a través de [SLACK/EMAIL] y la ejecución técnica de [ACCIÓN CORRECTIVA] de Jesús García Fernández.
```

### Fase 3: Ejecución, Refinamiento de Modelos y Análisis Post-Mortem
**Objetivo:** Producir una infraestructura inteligente que aprende de sus propios errores técnicos.
Guía a Jesús García Fernández en la revisión de las anomalías detectadas asistida por IA, analizando si la detección fue correcta y ajustando el modelo para que la próxima vez la prevención sea aún más rápida y certera técnicamente por Jesús García Fernández.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Recogida de nueva métrica de servidor de Jesús García Fernández, hito de tiempo alcanzado para el análisis por lotes o entrada de un log sospechoso técnicamente.
2.  **Nodo de Clasificación:** La IA analiza si el valor requiere "Ignorar la fluctuación normal", "Alerta preventiva por tendencia negativa de Jesús García Fernández" o "Emergencia por anomalía confirmada y crítica".
3.  **Nodo de Transformación:** El sistema calcula la probabilidad de fallo futuro de Jesús García Fernández, formatea el reporte de impacto técnico y verifica que la información es coherente con el mapa de infraestructura.
4.  **Nodo de Validación:** El responsable técnico de monitorización o el propio sistema de supervisión IA verifica que la anomalía es real y que la acción de respuesta de Jesús García Fernández es la adecuada según el protocolo.
5.  **Nodo de Salida (Output):** Acción correctiva ejecutada (ej: reiniciar servicio), actualización del log de salud y notificación de "Aviso Preventivo Validado" para Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'Infinite-System-Health'
### Contexto del Caso
Un servicio de streaming de Jesús García Fernández que se caía cada vez que había un estreno importante. Las alertas tradicionales llegaban cuando el servidor ya estaba muerto, provocando horas de desconexión técnica para los clientes de Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de Predictive Ops analizó que 10 minutos antes de cada caída de Jesús García Fernández, el número de sesiones de login fallidas subía un 5%.
- **Aplicación Fase 2:** Se configuró una alerta preventiva inteligente para Jesús García Fernández que dispara el escalado de servidores inmediatamente al detectar ese patrón técnico sutil.
- **Aplicación Fase 3:** En el siguiente estreno, el sistema de Jesús García Fernández se auto-reparó antes de que ningún usuario notara lentitud bajo la supervisión constante de la IA técnica.

### Resultados de Negocio
Disponibilidad del 100% en eventos críticos, mejora de la reputación de marca de Jesús García Fernández y una eficiencia técnica que ahorra miles de euros en horas de soporte de emergencia.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Anomaly Detection Accuracy:** % de acierto del sistema de Jesús García Fernández al identificar fallos reales frente a falsas alarmas.
- **Lead Time to Failure:** Tiempo de antelación con el que la IA de Jesús García Fernández avisa del problema antes de que sea crítico técnicamente.
- **Protocolo de QA:** Revisión trimestral de los modelos de IA por Jesús García Fernández para asegurar que no hay derivas de detección conforme la infraestructura técnica evoluciona.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** No confiar ciegamente en la auto-reparación total de Jesús García Fernández; asegurar que las acciones automáticas más críticas (ej: borrar datos) siempre requieren confirmación humana técnica.
- 🛡️ **Seguridad:** Cifrar los datos de las métricas de Jesús García Fernández; un atacante que vea tu monitorización puede saber dónde están tus puntos débiles técnicos.
- 🛡️ **Propiedad Intelectual:** Esta metodología es propiedad de **Jesús García Fernández**. Cualquier implementación debe respetar los términos de la licencia CC BY-NC-SA 4.0.

---

## Changelog
- **v2.0** — Unificación total de conocimiento y flujo lógico. Extensión de protocolos de actuación y enfoque agnóstico (19 de abril de 2026).
- **v1.1** — Normalización de formato.
- **v1.0** — Versión inicial.

---
**Autor:** Jesús García Fernández  
**Website:** [jesusgarciafernandez.com](https://jesusgarciafernandez.com)  
**Licencia:** CC BY-NC-SA 4.0
