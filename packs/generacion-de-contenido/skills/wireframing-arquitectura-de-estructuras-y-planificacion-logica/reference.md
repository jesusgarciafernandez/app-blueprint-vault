# Referencia ampliada — Wireframing, Arquitectura de Estructuras y Planificación Lógica

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de generación de estructuras automatizada.*

1.  **Trigger:** Entrega de un documento PRD (Product Requirements Document) en formato texto.
2.  **Nodo de Extracción de Componentes IA:** El sistema identifica los requisitos (ej: "Buscador de personas", "Filtro por fecha", "Botón de exportar").
3.  **Nodo de Layout Automático:** IA coloca los componentes en una rejilla estándar de 12 columnas siguiendo las leyes de UX (ej: Buscador arriba, CTAs a la derecha).
4.  **Nodo de Verificación de Jerarquía IA:** El sistema avisa si el botón de "Borrar" tiene el mismo peso visual que el de "Guardar".
5.  **Output:** Archivo de Figma con wireframes Lo-Fi iniciales generados, listos para ser refinados por el arquitecto de información.

---

## 7. Ejemplo Práctico: Dashboard de Logística
**Reto:** El cliente quería "muchos datos" en una pantalla, lo que generaba un desorden visual insoportable.
**Acción v2.0:** Se trabajó solo en wireframes. Se usaron cajas grises para agrupar los datos por temática (Geografía, Tiempos, Incidencias). Se eliminaron todos los colores. Se validó con los transportistas si encontraban el dato "Número de ruta" en < 2 segundos.
**Resultado:** Se descubrió que el 50% de los datos que pedía el cliente no se miraban nunca. Se eliminaron de la estructura, dejando un dashboard limpio y centrado en la acción que ahorró 3 semanas de diseño UI complejo.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
