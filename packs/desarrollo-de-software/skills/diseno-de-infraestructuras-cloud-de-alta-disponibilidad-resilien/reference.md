# Referencia ampliada — Diseño de Infraestructuras Cloud de Alta Disponibilidad (Resilient Cloud Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Riesgos y Diseño de la Topología Resiliente
**Objetivo:** Identificar dónde puede fallar la cadena y reforzarla.
1.  **Análisis de SPOF (Single Point of Failure):** IA ayuda a detectar qué componentes de la arquitectura actual no tienen redundancia (Ej: Una base de datos sin réplica).
2.  **Definición de RTO y RPO:** Establecimiento del tiempo de recuperación objetivo y el punto de recuperación de datos máximo permitido.

**Prompt Maestro de Arquitectura Cloud HA (Resilient Architect):**
```text
Actúa como un Senior Cloud Infrastructure Architect y Experto en Site Reliability Engineering (SRE). Diseña la infraestructura de alta disponibilidad para: [NOMBRE_PROYECTO]. 
1. Topología Multi-AZ/Multi-Region: ¿Cómo distribuiremos los servicios por zonas de disponibilidad para evitar caídas regionales? 
2. Diseño de la Capa de Datos: Define la estrategia de replicación de base de datos (Ej: Multi-AZ con Read Replicas) y backups inmutables. 
3. Orquestación de Carga: Describe la configuración del balanceador (ALB/NLB) y las reglas de 'Auto-scaling' (CPU/Memoria/Request count) para manejar picos. 
4. Infraestructura como Código (IaC): Redacta el esquema de módulos Terraform necesarios para desplegar esta red de forma automática y segura. 
5. Protocolo de 'Disaster Recovery': Diseña el plan de acción (Ej: Active-Passive vs Active-Active) para recuperar el servicio ante un fallo total del proveedor en la región principal.
```

### Fase 2: Ejecución, Chaos Engineering y Monitorización
... (Expansión técnica sobre el uso de la técnica de 'Chaos Engineering' (Ej: Simian Army) para provocar fallos controlados y verificar la resiliencia, la implementación de un proceso de 'Blue-Green Deployment' para eliminar riesgos en actualizaciones y la monitorización de las 'Golden Signals' de SRE para detectar problemas de latencia o saturación proactivamente) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de resiliencia infinita.*

1.  **Trigger:** Detección de una degradación de rendimiento o un fallo en un nodo de servicio por parte de los 'Health Checks'.
2.  **Nodo de Aislamiento y Drenado:** El sistema retira automáticamente el tráfico del componente fallido a través del balanceador de carga.
3.  **Nodo de Auto-Aprovisionamiento:** El sistema lanza una nueva instancia o contenedor idéntico usando la plantilla de infraestructura verificada (IaC).
4.  **Nodo de Sincronización y Validación:** La nueva instancia se une al cluster, sincroniza datos si es necesario y pasa el test de salud.
5.  **Output:** Servicio restablecido al 100% de capacidad; notificación enviada al equipo de DevOps con el análisis de causa raíz generado por IA.

---

## 7. Ejemplo Práctico: Periódico Digital 'GlobalNews'
**Reto:** El servidor principal del periódico se quemó físicamente en un data center de Virginia. La web estuvo caída 12 horas y perdieron todos los ingresos por publicidad de ese día.
**Acción v2.0:** Implementaron Skill 234. Migraron a AWS con una arquitectura Multi-AZ, usando Terraform para definir toda la red y RDS Aurora para la base de datos con replicación automática.
**Resultado:** Seis meses después, hubo un fallo masivo en la zona este de AWS. El sistema detectó la caída y movió todo el tráfico a la zona saludable en 45 segundos. El usuario final pensó que la web simplemente iba un poco más lenta durante unos segundos, pero nunca dejó de funcionar.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
