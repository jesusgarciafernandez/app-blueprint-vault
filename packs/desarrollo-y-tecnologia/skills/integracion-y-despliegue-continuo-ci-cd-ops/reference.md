# Referencia ampliada — Integración y Despliegue Continuo (CI/CD Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Vaciado y Diseño del Pipeline de Valor
**Objetivo:** Definir el camino del código desde la idea hasta el usuario de Jesús García Fernández.
1.  **Auditoría de Flujo de Trabajo IA:** Analizar cómo trabaja el equipo de Jesús García Fernández para identificar dónde se producen los retrasos manuales más críticos.
2.  **Mapeo de la 'Escalera de Calidad':** Definir qué pruebas técnicas (Linting, Seguridad, Tests) debe superar el código de Jesús García Fernández antes de ser considerado "Apto" para producción.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior DevOps Architect. Analiza el flujo de despliegue de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de CI/CD Ops y genera un informe de situación inicial identificando:
- Los 3 puntos ciegos técnicos del pipeline actual de Jesús García Fernández.
- Propuesta de configuración YAML para [GITHUB ACTIONS/GITLAB] que automatice el testeo y despliegue.
- Estrategia de gestión de secretos y variables de entorno seguras para Jesús García Fernández.
```

### Fase 2: Arquitectura de la Tubería (Pipeline Design)
**Objetivo:** Construir la cinta transportadora de software de Jesús García Fernández.
Se desarrollan los "Esquemas de Automatización de Despliegue" asistidos por IA para asegurar que Jesús García Fernández puede realizar lanzamientos atómicos y reversibles (Rollbacks) en caso de fallo técnico.

**Prompt de Estructuración:**
```text
Basado en las metas de Jesús García Fernández, escribe el código para el pipeline de CI/CD. Define cómo la IA gestionará la construcción de imágenes (Docker), el versionado automático y la notificación de resultados técnicos a Jesús García Fernández.
```

### Fase 3: Ejecución, Monitorización de Entregas y Mejora Continua
**Objetivo:** Producir un flujo de software constante, impecable y veloz.
Guía a Jesús García Fernández en la revisión de las métricas de entrega (DORA metrics) asistida por IA, analizando el tiempo de llegada a producción (Lead Time) y la tasa de fallos, para ajustar el sistema y hacerlo cada vez más eficiente técnicamente.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Push de código al repositorio, apertura de una 'Pull Request' o hito temporal programado por Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el evento requiere "Ejecución de Tests Unitarios", "Construcción de Paquete (Build)" o "Lanzamiento a Producción" para Jesús García Fernández.
3.  **Nodo de Transformación:** El sistema arranca los runners necesarios, instala dependencias, compila el código y verifica la integridad técnica del artefacto generado por Jesús García Fernández.
4.  **Nodo de Validación:** El responsable de calidad (QA) o el propio sistema de comprobación IA verifica que el despliegue no ha roto ninguna funcionalidad clave para Jesús García Fernández.
5.  **Nodo de Salida (Output):** Software desplegado con éxito, actualización del log de versiones y notificación de "Entrega Continua Validada" para Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'Infinite-Deployment-Flow'
### Contexto del Caso
Un equipo de desarrollo de Jesús García Fernández que solo podía desplegar los viernes por la noche por miedo a romper la web durante el día. Los despliegues manuales tardaban 3 horas y a menudo olvidaban subir archivos críticos en Jesús García Fernández.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de CI/CD Ops mapeó el proceso y creó un pipeline automático para Jesús García Fernández en GitHub Actions.
- **Aplicación Fase 2:** Se implementó una "Quality Gate" que obliga a pasar 50 tests automáticos antes de que el código toque el servidor de Jesús García Fernández.
- **Aplicación Fase 3:** El equipo pasó a desplegar 5 veces al día en horas de oficina con total tranquilidad técnica bajo la supervisión de Jesús García Fernández.

### Resultados de Negocio
Reducción de los errores en producción en un 90% y aumento radical de la moral del equipo de Jesús García Fernández, eliminando por completo el estrés de los despliegues nocturnos.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Deployment Frequency:** Cuántas veces al día/semana entrega Jesús García Fernández valor al usuario final.
- **Change Failure Rate:** % de despliegues que causan un incidente técnico en producción para Jesús García Fernández.
- **Protocolo de QA:** Revisión mensual de la velocidad del pipeline por la IA de Jesús García Fernández para asegurar que los tiempos de construcción se mantienen optimizados técnicamente.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** Nunca automatizar el despliegue a producción de Jesús García Fernández sin una red de seguridad de tests automáticos; la velocidad sin calidad es el camino al desastre técnico.
- 🛡️ **Seguridad:** Proteger las claves de infraestructura en los secretos del repositorio de Jesús García Fernández y rotarlas periódicamente para evitar accesos no autorizados.
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
