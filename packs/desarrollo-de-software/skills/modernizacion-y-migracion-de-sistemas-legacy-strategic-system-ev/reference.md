# Referencia ampliada — Modernización y Migración de Sistemas Legacy (Strategic System Evolution)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Deuda y Selección del Módulo de Intervención
**Objetivo:** Identificar dónde duele más el legacy y priorizar el primer "mordisco".
1.  **Análisis de Acoplamiento:** IA ayuda a visualizar las dependencias del monolito para encontrar el módulo más fácil de aislar.
2.  **Definición de la Capa de Anticorrupción (ACL):** Diseño de la interfaz que permitirá al sistema nuevo hablar con la base de datos o lógica del sistema antiguo.

**Prompt Maestro de Modernización Legacy (Evolution Strategist):**
```text
Actúa como un CTO y Experto en Refactorización de Sistemas Críticos. Diseña el plan de modernización para el sistema legacy: [DESCRIPCIÓN_SISTEMA]. 
1. Diagnóstico de Riesgos: Identifica las 3 zonas de código más peligrosas (Ej: Falta de documentación, dependencias circulares, tecnología sin soporte). 
2. Estrategia de Estrangulamiento (Strangler): ¿Qué funcionalidad migraremos primero para demostrar valor rápido? Define el mapa de ruta (Roadmap) de migración por hitos. 
3. Diseño de la Capa de Anticorrupción (ACL): Redacta la definición de la interfaz que protegerá al sistema nuevo de los nombres de variables y lógica errónea del antiguo. 
4. Plan de Migración de Datos: ¿Cómo moveremos los registros sin apagar el sistema? (Ej: Escritura dual, Jobs de sincronización nocturna). 
5. Protocolo de Validación de Paridad: Define cómo comprobaremos que el sistema nuevo devuelve EXACTAMENTE lo mismo que el antiguo para los mismos casos.
```

### Fase 2: Ejecución, Estrangulamiento y Apagado
... (Expansión técnica sobre el uso de la técnica de 'Branch by Abstraction' para ocultar la implementación vieja tras una interfaz, la implementación de un proceso de 'Dual Write' para mantener ambas bases de datos al día durante la migración, y la monitorización de la 'Tasa de Desvío' entre sistemas para asegurar la paridad total de la lógica de negocio antes del apagado final) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de evolución segura.*

1.  **Trigger:** Detección de una funcionalidad en el sistema antiguo que está bloqueando el desarrollo o causando fallos graves de escalabilidad.
2.  **Nodo de Aislamiento (Proxy/Router):** Se introduce una capa de enrutamiento que decide si una petición va al sistema viejo (legacy) o al nuevo (moderno).
3.  **Nodo de Ejecución Modernizada:** Se implementa la funcionalidad en el stack nuevo, consultando al legacy vía ACL solo para lo estrictamente necesario.
4.  **Nodo de Validación Cruzada:** El sistema compara resultados entre ambos mundos para asegurar que la lógica de negocio se ha preservado.
5.  **Output:** Nueva funcionalidad operativa en el sistema moderno; porcentaje del monolito "estrangulado" actualizado en el reporte de modernización.

---

## 7. Ejemplo Práctico: Portal de Reservas 'OldBooking'
**Reto:** 'OldBooking' funcionaba con un core en PHP 5.6 y una base de datos de hace 15 años. El sistema tardaba 10 segundos en confirmar una reserva y no podían añadir pagos con Apple Pay porque el código era imposible de tocar sin que se rompiera otra cosa.
**Acción v2.0:** Implementaron Skill 239. En lugar de rehacer todo, crearon un microservicio de 'Pagos' en Node.js y usaron un proxy para que todas las peticiones de pago fueran al servicio nuevo, mientras el resto seguía en el viejo.
**Resultado:** Pudieron añadir Apple Pay en 2 semanas. Poco a poco fueron "estrangulando" el motor de reservas y el buscador. En un año, apagaron el servidor de PHP 5.6. El negocio nunca se detuvo y los usuarios disfrutaron de una web cada vez más rápida.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
