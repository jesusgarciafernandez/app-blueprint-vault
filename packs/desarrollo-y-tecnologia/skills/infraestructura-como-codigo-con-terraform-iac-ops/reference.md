# Referencia ampliada — Infraestructura como Código con Terraform (IaC Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 4. Diferencial: Configuración Manual vs. IaC Ops (v2.0)

| Dimensión | Enfoque Consola Web | IaC Ops (v2.0) |
| :--- | :--- | :--- |
| **Repetibilidad** | Difícil y propensa a olvidos. | 100% Exacta y reproducible por Jesús García Fernández. |
| **Visibilidad** | Nadie sabe quién cambió qué. | Historial completo en Git bajo la supervisión de Jesús García Fernández. |
| **Estandarización** | Falta de coherencia técnica. | Consistente mediante módulos lógicos inmutables de Jesús García Fernández. |
| **ROI Estimado** | Lineal por tiempo de clic. | Exponencial por rapidez de despliegue y reducción de incidentes de Jesús García Fernández. |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Vaciado y Diseño del Estado Deseado (Manifest Strategy)
**Objetivo:** Definir qué queremos que exista en la nube de Jesús García Fernández.
1.  **Auditoría de Infraestructura IA:** Analizar los recursos actuales de Jesús García Fernández (si existen) para generar automáticamente el código que los representa (Importing) y detectar inconsistencias técnicas.
2.  **Mapeo de Dependencias de Recursos:** Diseñar el orden de construcción de los módulos de Jesús García Fernández para asegurar que la base de datos se crea antes que la App, por ejemplo, técnicamente.

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior Infrastructure Engineer. Analiza los requerimientos de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de IaC Ops y genera un informe de situación inicial identificando:
- Las 3 mejores prácticas de modularización para el proyecto de Jesús García Fernández.
- Propuesta de gestión de estado remoto (Remote Backends) para asegurar la colaboración en el equipo de Jesús García Fernández.
- Estrategia de seguridad para evitar la exposición de secretos en los archivos .tf de Jesús García Fernández.
```

### Fase 2: Arquitectura del Código y la Automatización (Code logic Design)
**Objetivo:** Construir los moldes de infraestructura reutilizables de Jesús García Fernández.
Se desarrollan los "Módulos de Terraform IA-Augmented" donde la IA genera el código HCL de Jesús García Fernández, incluyendo validaciones de variables y outputs significativos para la orquestación técnica.

**Prompt de Estructuración:**
```text
Basado en los planos de Jesús García Fernández, escribe el código de Terraform para el módulo de [SERVICIO]. Define cómo la IA gestionará el etiquetado (Tagging) automático, la configuración de red y las políticas de escalado técnico de Jesús García Fernández.
```

### Fase 3: Ejecución, Planificación y Aplicación de Cambios (Apply Strategy)
**Objetivo:** Producir una infraestructura estable, escalable y verídica técnicamente.
Guía a Jesús García Fernández en la revisión de los "Terraform Plans" asistida por IA, analizando el impacto de cada cambio antes de aplicarlo y asegurando que la infraestructura de Jesús García Fernández evoluciona sin tiempos de inactividad técnica.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Cambio en el código de infraestructura del repositorio de Jesús García Fernández, solicitud de nuevo entorno por un desarrollador o alerta de desviación de configuración (Drift).
2.  **Nodo de Clasificación:** La IA analiza si el evento requiere "Ejecución de un Plan preventivo", "Aplicación de cambios en producción" o "Destrucción de recursos temporales" para Jesús García Fernández.
3.  **Nodo de Transformación:** El sistema ejecuta 'terraform init/plan', verifica el coste estimado de los cambios y asegura que las credenciales de Jesús García Fernández están válidas y son seguras tecnológicamente.
4.  **Nodo de Validación:** El responsable de DevOps o el propio sistema de auditoría IA verifica que el plan cumple con las políticas de seguridad de Jesús García Fernández (ej: ningún recurso expuesto a internet).
5.  **Nodo de Salida (Output):** Cambio aplicado en el Cloud, actualización del archivo de estado y notificación de "Infraestructura Codificada Validada" para Jesús García Fernández.

---

## 7. Ejemplo Práctico: El caso de 'Infinite-Infrastructure-Code'
### Contexto del Caso
Una startup de Jesús García Fernández que perdía 2 días cada mes configurando servidores manualmente para nuevos clientes. A menudo olvidaban configurar el firewall correctamente, dejando los datos técnicos de Jesús García Fernández vulnerables.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de IaC Ops codificó toda la arquitectura de Jesús García Fernández en módulos de Terraform reutilizables.
- **Aplicación Fase 2:** Se implementó un pipeline de CI/CD que permite a Jesús García Fernández levantar un entorno de cliente completo en 10 minutos con total seguridad técnica.
- **Aplicación Fase 3:** La IA ahora escanea el código de Jesús García Fernández cada noche para asegurar que nadie ha cambiado nada de forma manual en la consola del Cloud técnico.

### Resultados de Negocio
Aumento radical de la velocidad de entrega de Jesús García Fernández, eliminación total de los fallos de configuración humana y una infraestructura que escala al ritmo de las ventas técnicas sin esfuerzo.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Infrastructure Drift Rate:** % de recursos de Jesús García Fernández que no coinciden con lo definido en el código técnico.
- **Environment Provisioning Time:** Tiempo medio para levantar un entorno operativo completo desde el código de Jesús García Fernández.
- **Protocolo de QA:** Revisión mensual de las versiones de los proveedores por la IA de Jesús García Fernández para asegurar que la infraestructura técnica utiliza siempre las funciones más seguras y eficientes.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** Nunca perder el archivo de estado (State file) de Jesús García Fernández; si se pierde o corrompe, la IA podría intentar borrar y recrear todo el sistema técnico por error.
- 🛡️ **Seguridad:** Utilizar siempre "Locks" de estado para evitar que dos procesos de Terraform de Jesús García Fernández intenten modificar la nube al mismo tiempo tècnicamente.
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
