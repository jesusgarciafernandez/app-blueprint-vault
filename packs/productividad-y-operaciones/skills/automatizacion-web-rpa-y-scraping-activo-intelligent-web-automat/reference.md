# Referencia ampliada — Automatización Web RPA y Scraping Activo (Intelligent Web Automation)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Fuentes y Diseño del Flujo de Interacción
**Objetivo:** Obtener los datos de forma ética, rápida y sin ser detectado.
1.  **Análisis de la 'Huella Digital' del Objetivo:** IA ayuda a identificar qué medidas de protección usa la web (Ej: Cloudflare, Akamai) y diseña la estrategia de bypass.
2.  **Mapeo del Flujo RPA:** Definición de los pasos exactos que el bot debe seguir (Ej: Login -> Click en 'Informes' -> Selección de fecha -> Descarga).

**Prompt Maestro de RPA & Scraping (Digital Miner Architect):**
```text
Actúa como un Senior Automation Engineer y Experto en Web Scraping Avanzado. Diseña el sistema de recolección de datos para: [URL_OBJETIVO]. 
1. Arquitectura de Navegación: ¿Usaremos Playwright Headless o con UI? Define la estrategia de rotación de proxies y User-Agents para evitar el bloqueo. 
2. Selección de Datos (Selectores Robustos): Identifica los 5 puntos de datos críticos y propón selectores XPath/CSS que sean resistentes a cambios en el layout de la página. 
3. Lógica RPA de Interacción: Redacta el script lógico para manejar [ACCIÓN_COMPLEJA] (Ej: Loguearse, superar un Captcha simple y navegar a través de un scroll infinito). 
4. Pipeline de Limpieza: ¿Cómo transformaremos el texto extraído (RAW) en un formato estructurado y validado (Ej: JSON Schema)? 
5. Gestión de Errores y Retries: Define el protocolo de reintento si la red falla o si el selector no se encuentra (Exponential Backoff).
```

### Fase 2: Ejecución, Escalamiento y Orquestación de Datos
... (Expansión técnica sobre el uso de la técnica de 'Browser Context' para aislar sesiones, la implementación de un proceso de 'Distributed Scraping' para grandes volúmenes de datos, y la monitorización de la 'Tasa de Bloqueo' para ajustar la evasión dinámicamente) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de minería digital.*

1.  **Trigger:** Evento programado (cron) o solicitud manual de recolección de datos específicos.
2.  **Nodo de Inicialización de Entorno:** El sistema levanta un navegador con una identidad digital limpia (Proxy, UA, Cookies).
3.  **Nodo de Ejecución RPA:** El bot navega por la web objetivo, realiza las interacciones necesarias y extrae la información del DOM.
4.  **Nodo de Validación y Estructuración:** Los datos brutos se limpian, se eliminan duplicados y se validan contra el esquema de negocio.
5.  **Output:** Base de datos o archivo listo para consumo humano o IA; reporte de éxito y estadísticas de recolección generado.

---

## 7. Ejemplo Práctico: Comparador de Viajes 'FlyCheap'
**Reto:** 'FlyCheap' necesitaba actualizar el precio de sus ofertas cada 10 minutos desde 20 webs diferentes de aerolíneas que no tienen API abierta y bloquean activamente el scraping.
**Acción v2.0:** Implementaron Skill 252. Desarrollaron una red de bots con Playwright que utilizan proxys residenciales y simulan movimientos de ratón humanos para navegar por las aerolíneas.
**Resultado:** Ahora obtienen precios actualizados al segundo con una tasa de éxito del 98%. Han superado a competidores más grandes que solo actualizan una vez al día, convirtiéndose en la web de referencia para chollos de última hora.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
