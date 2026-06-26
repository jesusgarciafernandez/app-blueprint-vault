# Referencia ampliada — Desarrollo WordPress Avanzado y Seguro (Enterprise CMS Engineering)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría Técnica y Diseño de la Arquitectura de Seguridad
**Objetivo:** Establecer una base técnica inexpugnable y de alto rendimiento.
1.  **Auditoría de Plugins y Performance:** IA ayuda a detectar qué plugins están ralentizando el sitio y propone alternativas de micro-código a medida.
2.  **Plan de Hardening:** Definición de las directivas de seguridad en `.htaccess`, `nginx.conf` y `wp-config.php`.

**Prompt Maestro de Ingeniería WordPress (CMS Architect):**
```text
Actúa como un Senior WordPress Developer y Experto en Ciberseguridad Web. Diseña la arquitectura avanzada para el sitio: [DOMINIO/PROYECTO]. 
1. Estrategia de Desarrollo a Medida: ¿Cómo estructuraremos el 'Custom Theme' para evitar la dependencia de constructores visuales pesados (Ej: Elementor/Divi)? 
2. Plan de Seguridad Proactiva: Redacta las 5 reglas de seguridad más críticas que inyectaremos en el servidor para bloquear ataques de fuerza bruta y XML-RPC. 
3. Optimización de Base de Datos y Caché: Describe la configuración de Redis y cómo optimizaremos las consultas 'wp_query' pesadas para mejorar el TTFB. 
4. Implementación de SEO Técnico: Define la estrategia de datos estructurados (JSON-LD) y cómo aseguraremos una puntuación de 90+ en Core Web Vitals. 
5. Flujo de Despliegue Seguro (Staging to Prod): Diseña el proceso para probar cambios en un entorno espejo antes de sincronizar la base de datos con producción.
```

### Fase 2: Ejecución, Optimización y Blindaje Continuo
... (Expansión técnica sobre el uso de la técnica de 'Headless WordPress' para separar el diseño de la lógica, la implementación de un proceso de 'Object Caching' para reducir la carga de la base de datos, y la monitorización de la 'Integridad de Archivos' para detectar archivos inyectados o modificaciones no autorizadas en tiempo real) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de robustez digital.*

1.  **Trigger:** Lanzamiento de un nuevo sitio WordPress o necesidad de securizar/optimizar uno existente.
2.  **Nodo de Escaneo y Diagnóstico:** El sistema analiza la salud actual del sitio, detectando vulnerabilidades de plugins e ineficiencias de carga.
3.  **Nodo de Inyección de Lógica Avanzada:** Se aplican las configuraciones de seguridad core y se sustituyen plugins genéricos por funciones optimizadas en `functions.php`.
4.  **Nodo de Verificación de Performance:** El sistema realiza un benchmark de velocidad y SEO, ajustando la configuración de caché y entrega de activos.
5.  **Output:** Sitio WordPress blindado, ultra-rápido y optimizado para SEO; reporte de seguridad e integridad disponible para el administrador.

---

## 7. Ejemplo Práctico: Revista Digital 'EcoTrend'
**Reto:** 'EcoTrend' sufría caídas constantes cuando sus noticias se hacían virales, y su panel de administración estaba siendo atacado por bots continuamente. La web tardaba 6 segundos en cargar.
**Acción v2.0:** Implementaron Skill 244. Eliminaron 15 plugins innecesarios sustituyéndolos por código puro, movieron la web a un stack con Nginx y Redis, y blindaron el acceso a `/wp-admin`.
**Resultado:** El tiempo de carga bajó a 800ms. Durante la última viralidad con 50.000 visitas simultáneas, el servidor apenas se inmutó. Los intentos de ataque ahora son bloqueados automáticamente en el borde antes de tocar WordPress.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
