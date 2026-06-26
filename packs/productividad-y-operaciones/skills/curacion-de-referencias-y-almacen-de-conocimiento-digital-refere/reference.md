# Referencia ampliada — Curación de Referencias y Almacén de Conocimiento (Digital Reference Curation)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Fuentes y Diseño del Flujo de Captura
**Objetivo:** Crear un proceso de un solo click que no interrumpa el flujo de trabajo.
1.  **Centralización del Punto de Entrada:** Definir un único lugar (Ej: Raindrop) donde va todo lo que se encuentra en la web antes de ser procesado.
2.  **Mapeo de la Taxonomía PARA:** IA ayuda a clasificar los favoritos actuales en las 4 macro-categorías (Proyectos, Áreas, Recursos, Archivos).

**Prompt Maestro de Curación Referencial (Reference Architect):**
```text
Actúa como un Senior Knowledge Manager y Experto en PKM (Personal Knowledge Management). Diseña el sistema de referencias para el área: [TEMA/PROYECTO]. 
1. Arquitectura de Etiquetas (Tagging System): Propón 10 etiquetas jerárquicas que describan el estado de la referencia (Ej: #ParaLeer, #UtilidadDirecta, #Inspiración). 
2. Flujo de Metabolización: ¿Cómo pasará un artículo de ser una 'URL guardada' a un 'Concepto Integrado' en mi base de conocimiento (Ej: Raindrop -> Readwise -> Notion)? 
3. Sistema de Filtros de Calidad: Define los 3 criterios de 'Corte' para que un enlace merezca ser guardado en la biblioteca permanente (Recurso/Archivo). 
4. Automatización de Resúmenes: Describe cómo usaremos la IA para extraer los 'Puntos de Acción' de cada página web guardada de forma automática. 
5. Protocolo de Auditoría Trimestral: Diseña el checklist para limpiar los enlaces rotos y mover los proyectos cerrados al área de 'Archivos'.
```

### Fase 2: Ejecución, Digestión de Conocimiento y Jardinería Digital
... (Expansión técnica sobre el uso de la técnica de 'Progressive Summarization' para extraer capas de valor de un texto, la implementación de un proceso de 'Cross-linking' para conectar referencias de diferentes temas, y la monitorización de la 'Tasa de Uso' de las referencias para asegurar que el sistema es productivo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de inspiración accesible.*

1.  **Trigger:** El usuario encuentra un recurso valioso en la red y activa el capturador (Extension/App).
2.  **Nodo de Pre-clasificación por IA:** El sistema analiza el contenido de la URL, extrae metadatos, sugiere etiquetas y asigna una categoría PARA inicial.
3.  **Nodo de Síntesis y Resaltado:** Si el usuario lee el recurso, los fragmentos subrayados se extraen automáticamente y se envían a la base de conocimiento central.
4.  **Nodo de Vinculación de Proyecto:** El sistema detecta si la referencia es relevante para un proyecto activo y la muestra en el panel de control correspondiente.
5.  **Output:** Biblioteca de referencias enriquecida; conocimiento curado y disponible; inspiración lista para ser transformada en acción.

---

## 7. Ejemplo Práctico: El 'Swiper' Inmobiliario
**Reto:** Un agente inmobiliario pasaba 2 horas al día buscando noticias del sector, ejemplos de contratos y webs de la competencia, pero cuando llegaba el momento de preparar una oferta, nunca encontraba aquel "artículo tan bueno" que había leído hace un mes.
**Acción v2.0:** Implementó Skill 259. Usa Raindrop para guardar todo con etiquetas visuales (#Contratos, #Tendencias2024, #Competencia). La IA de Raindrop le resume los artículos largos y los conecta con sus páginas de cliente en Notion.
**Resultado:** Ahora tarda 5 segundos en encontrar cualquier referencia. Ha creado una biblioteca de "Casos de éxito" visuales que enseña a sus clientes en el iPad, cerrando ventas mucho más rápido al demostrar que está a la vanguardia de la información del sector.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
