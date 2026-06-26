# Referencia ampliada — Validación Visual de Interfaces (Visual Regression Testing & UI Integrity)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Superficie Visual y Definición de Estados
**Objetivo:** Crear una base de referencia visual perfecta.
1.  **Mapeo de 'Páginas Semilla':** IA ayuda a identificar las pantallas con mayor densidad de componentes y variaciones de layout para testear.
2.  **Configuración de la Matriz de Dispositivos:** Definición de los 'Viewports' críticos (Ej: iPhone 15, iPad Pro, Desktop 4K) para las capturas.

**Prompt Maestro de Visual QA (Aesthetic Engineer):**
```text
Actúa como un Senior UI/UX Engineer y Experto en Visual Regression Testing. Diseña la estrategia de validación visual para el proyecto: [NOMBRE_PROYECTO]. 
1. Matriz de Snapshots: Define las 5 pantallas críticas y los 3 estados de componente (Ej: Default, Hover, Active) que deben ser capturados obligatoriamente. 
2. Configuración de Playwright Visual: Redacta el código para una prueba que haga scroll, espere a las fuentes y capture una 'Full Page Snapshot' sin ruido de elementos dinámicos (Ej: fechas, banners). 
3. Umbral de Tolerancia (Mismatch Threshold): Justifica el porcentaje de diferencia permitido (Ej: 0.1%) para evitar falsos positivos por renderizado de fuentes o bordes difusos. 
4. Estrategia de 'Frozen States': Describe cómo congelaremos animaciones, ocultaremos cursores y fijaremos fechas para que los snapshots sean deterministas. 
5. Flujo de Aprobación Documental: Redacta el protocolo para que el equipo de diseño valide visualmente los cambios detectados en la PR antes de subir el código.
```

### Fase 2: Ejecución, Revisión de Mismatches y Mejora Continua
... (Expansión técnica sobre el uso de la técnica de 'Dynamic Content Masking' para ignorar áreas con datos variables en las fotos, la implementación de un proceso de 'Cross-browser Visual Check' para detectar fallos específicos de Safari o Edge, y la monitorización de la 'Integridad Visual' en el tiempo para asegurar que el sistema de diseño no se degrada con el uso) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de perfección visual.*

1.  **Trigger:** El desarrollador envía código al repositorio que modifica componentes de UI o archivos de estilos (CSS/SCSS).
2.  **Nodo de Ejecución de Capturas:** El sistema levanta la app en contenedores aislados y toma fotos de alta resolución en la matriz de dispositivos definida.
3.  **Nodo de Comparación Biónica:** Una IA de comparación visual analiza las fotos actuales contra la 'Baseline' aprobada, resaltando las diferencias en rojo.
4.  **Nodo de Alerta Estética:** Si hay diferencias, se bloquea la PR y se presenta un 'Visual Diff Viewer' interactivo para revisión humana.
5.  **Output:** Si el humano aprueba, la nueva foto se convierte en la nueva 'Baseline'; si rechaza, el desarrollador debe corregir el estilo del código.

---

## 7. Ejemplo Práctico: Periódico de Diseño 'TheArtPost'
**Reto:** 'TheArtPost' es una web de diseño donde la tipografía y los espacios en blanco son sagrados. Un desarrollador cambió una variable de margen en el footer y, sin querer, desplazó 2 píxels todo el contenido lateral en el iPad, arruinando la elegancia del sitio durante días.
**Acción v2.0:** Implementaron Skill 242. Crearon un pipeline con Percy que saca fotos de cada sección en cada commit.
**Resultado:** Cuando el desarrollador intentó hacer de nuevo un cambio "pequeño" en el CSS, el sistema detectó la desviación de 2 píxels en el iPad inmediatamente. El cambio fue rechazado automáticamente antes de llegar a producción, salvaguardando la reputación estética del periódico.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
