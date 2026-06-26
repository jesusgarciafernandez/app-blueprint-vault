# Referencia ampliada — Optimización de Flujos de Trabajo (Workflow Engineering & Lean Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Flujo y Detección de Fricción
**Objetivo:** Identificar dónde se detiene el valor y por qué.
1.  **Value Stream Mapping (VSM):** IA ayuda a documentar cada paso del proceso, separando las tareas que añaden valor de las que son puramente administrativas o de espera.
2.  **Identificación del 'Cuello de Botella' (Constraint):** Localización del punto exacto que limita la velocidad de todo el sistema.

**Prompt Maestro de Optimización de Flujos (Workflow Architect):**
```text
Actúa como un Senior Operations Consultant y Experto en Lean Manufacturing aplicado a Servicios Digitales. Optimiza el flujo de trabajo: [NOMBRE_FLUJO]. 
1. Mapeo As-Is (Estado Actual): Identifica los 3 pasos donde se produce el mayor 'Lead Time' (espera) y las causas probables (Ej: Aprobación manual, falta de datos). 
2. Rediseño To-Be (Estado Optimizado): Propón un nuevo flujo que elimine 2 pasos redundantes y automatice el 'Hand-off' entre [ROL_A] y [ROL_B]. 
3. Definición de KPIs de Flujo: Establece los objetivos de 'Cycle Time' para cada fase y el 'Throughput' (capacidad de salida) esperado tras la optimización. 
4. Implementación de 'Quick Wins': ¿Qué pequeño cambio tecnológico (Ej: Una regla de Slack, un template) podemos aplicar hoy para mejorar la fluidez un 20%? 
5. Plan de Monitorización de Salud del Proceso: Diseña un dashboard simple que alerte si una tarea lleva parada más tiempo del estándar definido.
```

### Fase 2: Ejecución, Pilotaje de Automatización y Ajuste Continuo
... (Expansión técnica sobre el uso de la técnica de 'Kanban Systems' para visualizar el trabajo en curso (WIP), la implementación de un proceso de 'Poka-Yoke' digital para evitar errores en la entrada de datos, y la monitorización de la 'Tasa de Valor Agregado' para asegurar que el proceso se mantiene ligero y eficiente en el tiempo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de fluidez total.*

1.  **Trigger:** Detección de un retraso sistemático en un proceso o inicio de un proyecto de mejora operativa.
2.  **Nodo de Análisis de Trazabilidad:** El sistema recolecta datos de tiempos reales de ejecución y detecta anomalías o cuellos de botella automáticos.
3.  **Nodo de Rediseño Sugerido:** La IA propone una reconfiguración del flujo, sugiriendo la eliminación de pasos o la inserción de automatizaciones No-code.
4.  **Nodo de Implementación y Test de Carga:** Se despliega el nuevo flujo en un entorno controlado y se verifica su impacto en el 'Cycle Time'.
5.  **Output:** Flujo de trabajo optimizado y en marcha; manual de proceso actualizado automáticamente; dashboard de métricas de flujo activo para el líder de operaciones.

---

## 7. Ejemplo Práctico: Despacho Legal 'LegalFast'
**Reto:** 'LegalFast' tardaba 3 semanas en dar de alta a un nuevo cliente porque la información viajaba en hilos de email cruzados, se perdían documentos y los abogados no sabían cuándo podían empezar a trabajar. El desorden causaba estrés y pérdida de clientes.
**Acción v2.0:** Implementaron Skill 251. Mapearon el flujo de valor y descubrieron que el 70% del tiempo era "espera de correo". Crearon un formulario centralizado que dispara tareas automáticas y mueve los documentos a carpetas compartidas sin intervención humana.
**Resultado:** El tiempo de alta bajó de 21 días a 48 horas. El personal administrativo recuperó el 50% de su tiempo y los abogados empezaron a facturar antes. La satisfacción del cliente subió drásticamente al recibir un servicio rápido y profesional desde el minuto uno.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
