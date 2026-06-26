# Referencia ampliada — Estrategias de Testing de Aplicaciones Web (Elite Quality Assurance)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Cobertura y Diseño de la Estrategia
**Objetivo:** Identificar los "Caminos Críticos" que necesitan blindaje inmediato.
1.  **Mapeo de Flujos Críticos de Usuario:** IA ayuda a priorizar qué partes de la app (Ej: Login, Pago, Registro) deben tener tests E2E obligatorios.
2.  **Definición de Stack de Testing:** Selección de las herramientas óptimas según el framework de desarrollo (Ej: Jest para lógica, Playwright para UI).

**Prompt Maestro de QA Engineering (Trust Architect):**
```text
Actúa como un Senior QA Automation Engineer y Experto en Calidad de Software. Diseña la estrategia de testing para el proyecto: [NOMBRE_PROYECTO]. 
1. Estructura de la Pirámide: Define el porcentaje de cobertura objetivo para Unit, Integration y E2E. Justifica la distribución basándote en la velocidad y el coste. 
2. Diseño de Test E2E (Playwright): Redacta un script de ejemplo que verifique el flujo de [ACCION_CRITICA] en Chrome, Firefox y Safari, incluyendo esperas inteligentes. 
3. Estrategia de Mocking: ¿Cómo simularemos las respuestas de la API [API_X] para que los tests de frontend sean rápidos e independientes del backend? 
4. Check de Accesibilidad: Describe cómo integraremos 'axe-core' en el pipeline para detectar automáticamente fallos de contraste o etiquetas ARIA faltantes. 
5. Configuración de CI Quality Gate: Redacta el archivo YAML de GitHub Actions que ejecute los tests en cada Pull Request y bloquee el merge si fallan.
```

### Fase 2: Ejecución, Mantenimiento de Tests y Observabilidad
... (Expansión técnica sobre el uso de la técnica de 'Snapshot Testing' para detectar cambios inesperados en la UI, la implementación de un proceso de 'Flaky Test Detection' para eliminar pruebas inestables que causan ruido en el equipo, y la monitorización de la 'Cobertura de Código' (Coverage) para asegurar que las nuevas funcionalidades siempre nazcan con sus tests correspondientes) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de calidad absoluta.*

1.  **Trigger:** El desarrollador envía una solicitud de cambio (Commit/PR) al repositorio de código.
2.  **Nodo de Ejecución de Lests Unitarios:** El sistema lanza automáticamente los tests de lógica pura (velocidad < 1s por test).
3.  **Nodo de Despliegue en Entorno Efímero:** Se levanta una versión temporal de la web para ejecutar las pruebas de integración y E2E.
4.  **Nodo de Simulación de Usuario (E2E):** Un robot interactúa con la web real verificando que los botones, formularios y datos se comportan como se espera.
5.  **Output:** Reporte de calidad generado; si todo es verde, se autoriza el despliegue a producción; si algo falla, se notifica al autor con capturas y videos del error.

---

## 7. Ejemplo Práctico: E-commerce de Lujo 'LuxStore'
**Reto:** 'LuxStore' perdía miles de euros cada vez que el botón de "Añadir al Carrito" dejaba de funcionar tras una actualización de diseño. Los errores solo se detectaban cuando los clientes se quejaban por redes sociales.
**Acción v2.0:** Implementaron Skill 240. Crearon un conjunto de tests E2E con Playwright que verifica el flujo de compra cada vez que un diseñador toca el código.
**Resultado:** Ahora, si un cambio en el CSS oculta el botón de compra o rompe el JavaScript, el pipeline de CI/CD detecta el error en 3 minutos y detiene el lanzamiento. Cero errores de compra en producción durante los últimos 6 meses.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
