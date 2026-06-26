# Referencia ampliada — Diseño de Pipelines de Despliegue Continuo (CI/CD Automation)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría del Workflow actual y Diseño del Pipeline
**Objetivo:** Crear una ruta de despliegue sin fricciones y segura.
1.  **Mapeo del Flujo de Entrega:** IA ayuda a identificar dónde se pierde más tiempo (waiting times) en el proceso de desarrollo actual.
2.  **Definición de 'Quality Gates':** Establecimiento de los umbrales de éxito (Ej: 80% cobertura de tests, 0 vulnerabilidades críticas) para permitir el avance del código.

**Prompt Maestro de Diseño CI/CD (DevOps Engineer):**
```text
Actúa como un Senior DevOps Engineer y Experto en Automatización de Software. Diseña el pipeline de CI/CD para el proyecto: [NOMBRE_PROYECTO]. 
1. Arquitectura del Pipeline: Divide el flujo en etapas claras (Build, Test, Scan, Deploy) y define los disparadores (Triggers) para cada una (Push, PR, Merge). 
2. Definición de la Etapa de Testing: ¿Qué tipos de pruebas ejecutaremos y cómo integraremos el reporte de resultados en la interfaz del desarrollador? 
3. Estrategia de Contenerización: Redacta un Dockerfile multi-stage optimizado para este proyecto y describe el flujo de subida al registro de imágenes. 
4. Despliegue Continuo (CD): Diseña el método de actualización en producción (Ej: Rolling update en Kubernetes) y cómo manejaremos los secretos y variables de entorno. 
5. Protocolo de 'Rollback' Automático: Define la condición (Ej: Aumento de errores 5xx > 5%) que activará la vuelta atrás inmediata a la versión estable anterior.
```

### Fase 2: Ejecución, Monitorización de Pipelines y Optimización
... (Expansión técnica sobre el uso de la técnica de 'Build Caching' para reducir el tiempo de ejecución del pipeline, la implementación de un proceso de 'Pre-commit Hooks' para evitar que el código erróneo llegue siquiera al servidor de CI, y la monitorización de la 'Frecuencia de Despliegue' y el 'Change Failure Rate' (Métricas DORA) para medir la salud del proceso de entrega) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de entrega fluida.*

1.  **Trigger:** El desarrollador realiza un 'Merge' de una rama de funcionalidad verificada a la rama principal (Main/Master).
2.  **Nodo de Integración Continua (CI):** El sistema lanza el pipeline, compila el código, ejecuta los tests y realiza el análisis estático de seguridad en paralelo.
3.  **Nodo de Construcción de Artefacto:** Si los tests pasan, se crea una imagen de contenedor inmutable etiquetada con el ID del commit y se sube al registro privado.
4.  **Nodo de Despliegue Progresivo (CD):** El sistema actualiza el entorno de producción siguiendo la estrategia definida (Ej: Canary), monitorizando la salud del sistema durante el cambio.
5.  **Output:** Nueva versión disponible para los usuarios; reporte de despliegue exitoso enviado a los canales de comunicación del equipo de desarrollo.

---

## 7. Ejemplo Práctico: Aplicación de Delivery 'QuickEat'
**Reto:** Lanzar una actualización en 'QuickEat' era un evento traumático de 4 horas que requería que 5 ingenieros estuvieran conectados por la noche verificando que todo funcionaba. A menudo tenían que revertir cambios a mano tras fallos inesperados.
**Acción v2.0:** Implementaron Skill 235 con GitHub Actions y Kubernetes. Automatizaron el flujo completo desde el código hasta el deploy 'Canary' (lanzar al 10% de usuarios primero).
**Resultado:** Ahora los despliegues ocurren a mediodía, automáticamente tras el merge, y tardan 8 minutos. Si la IA de monitorización detecta anomalías en el 10% inicial, el sistema hace 'Rollback' solo en 15 segundos sin que el 90% de los usuarios se enteren de que hubo un problema.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
