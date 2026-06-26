# Referencia ampliada — Panel de Administración Master (Backoffice & Business Intelligence)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de KPIs y Diseño de la Estructura de Navegación
**Objetivo:** Reducir el tiempo de búsqueda para aumentar el tiempo de decisión.
1.  **Identificación de las 'Constantes Vitales' del Negocio:** IA ayuda a jerarquizar qué 4 métricas deben estar siempre visibles (Ej: Revenue, Active Sessions, Errors, Conversions).
2.  **Arquitectura de Permisos (RBAC):** Definición de qué puede ver cada rol (Admin, Editor, Support, Auditor) para garantizar el mínimo privilegio.

**Prompt Maestro de Diseño de Backoffice (Operations Architect):**
```text
Actúa como un Senior Product Manager y Experto en UX de Herramientas Internas. Diseña el Panel Master para el proyecto: [NOMBRE_PROYECTO]. 
1. Jerarquía de Información (Dashboard): Define las 4 'Stat Cards' superiores y el gráfico principal (Ej: Línea de tiempo de ventas) que darán la visión de salud inmediata. 
2. Diseño de la Data Table Principal: Describe las columnas, filtros y acciones masivas (Ej: Ban de usuarios, Enviar cupón) necesarias para gestionar la entidad [ENTIDAD_X]. 
3. Flujo de Navegación y Roles: Diseña el sidebar con secciones claras (Métricas, Usuarios, Configuración, Logs) y especifica qué rol accede a cada una. 
4. Implementación de Alertas Visuales: Propón un sistema de código de colores o iconos que resalte anomalías críticas (Ej: Caída de ventas > 20% en una hora) de forma instantánea. 
5. Protocolo de Auditoría: Define qué eventos (Quién, Cuándo, Qué) deben quedar registrados permanentemente para cumplir con la trazabilidad operativa.
```

### Fase 2: Ejecución, Refinamiento de Carga y Dashboards Interactivos
... (Expansión técnica sobre el uso de la técnica de 'Infinite Streaming' para tablas de gran tamaño, la implementación de un proceso de 'Real-time Updates' vía WebSockets o suscripciones de base de datos, y la monitorización de la 'Latencia de Dashboards' para asegurar que el panel nunca sea un cuello de botella para la rapidez de la organización) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control total.*

1.  **Trigger:** El administrador accede al backoffice o se dispara una alerta automática por una métrica fuera de rango.
2.  **Nodo de Agregación de Datos en Tiempo Real:** El sistema consulta las fuentes de verdad, aplica filtros de seguridad según el rol y genera los resúmenes estadísticos.
3.  **Nodo de Visualización Reactiva:** El panel presenta los datos mediante componentes premium (Charts/Tables) permitiendo la interacción profunda del humano.
4.  **Nodo de Acción Operativa:** El administrador realiza una acción manual o supervisa una automatización disparada por el sistema desde la misma interfaz.
5.  **Output:** Decisión estratégica ejecutada; estado de la plataforma modificado; registro de la acción guardado en el historial de auditoría maestro.

---

## 7. Ejemplo Práctico: App de Movilidad 'CityFlow'
**Reto:** Los gestores de 'CityFlow' no sabían en qué zonas de la ciudad faltaban patinetes hasta que recibían quejas. Consultaban manualmente 5 herramientas diferentes para entender la operativa del día anterior.
**Acción v2.0:** Implementaron Skill 005. Crearon un Panel Master con un mapa de calor en tiempo real y alertas de baja batería. Unificaron la gestión de usuarios y el soporte técnico en la misma herramienta.
**Resultado:** La eficiencia logística subió un 40%. Ahora los gestores mueven los patinetes proactivamente basándose en la predicción del dashboard. El tiempo de resolución de quejas de usuarios bajó de 2 horas a 10 minutos.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
