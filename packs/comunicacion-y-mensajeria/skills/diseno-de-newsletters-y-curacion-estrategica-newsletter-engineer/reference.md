# Referencia ampliada — Diseño de Newsletters y Curación Estratégica (Newsletter Engineering)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Nicho y Diseño de la Estructura Editorial
**Objetivo:** Definir qué vamos a decir y cómo lo vamos a organizar.
1.  **Definición de las 'Columnas del Contenido':** IA ayuda a identificar los 3-4 temas pilares que tratará la newsletter para asegurar la coherencia temática.
2.  **Diseño de la 'Skeleton-Template':** Creación de la estructura de secciones (Ej: Introducción Personal | Noticia de la Semana | Herramienta | Acción del Lector).

**Prompt Maestro de Diseño Editorial (Newsletter Architect):**
```text
Actúa como un Senior Editorial Director y Experto en Email Marketing Estratégico. Diseña el protocolo de la newsletter para: [NICHO/AUDIENCIA]. 
1. Arquitectura de Secciones: Define las 5 partes fijas del boletín que generen familiaridad y hábito en el lector. 
2. Guía de Tono y Voz: ¿Cómo hablaremos al suscriptor? (Ej: Mentor cercano, Analista riguroso, Comisario de arte) define el registro linguístico. 
3. Estrategia de Asuntos (Subject Lines): Propón 5 fórmulas de asuntos que despierten curiosidad sin ser clickbait y que aseguren un Open Rate >45%. 
4. Plan de Curación Inteligente: ¿Cómo usaremos herramientas (Ej: RSS, IA, Redes) para encontrar contenido de valor en menos de 1 hora semanal? 
5. Protocolo de Conversión Suave (Soft Sell): Define dónde y cómo inyectaremos las llamadas a la acción para nuestros productos sin romper la experiencia de lectura.
```

### Fase 2: Ejecución, Curación Semanal y Análisis de 'Deep Stats'
... (Expansión técnica sobre el uso de la técnica de 'Segmentación por Comportamiento', la implementación de un proceso de 'A/B Testing de Send-Times', y la monitorización de la 'Métrica de Crecimiento Orgánico' para asegurar que la newsletter se comparte por su propio valor intrínseco) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica editorial asistida.*

1.  **Trigger:** Finalización del proceso de curación semanal o recogida automática de enlaces de interés durante la semana en un repositorio central.
2.  **Nodo de Redacción de Borradores por IA:** El sistema toma los enlaces y notas del humano y genera un borrador estructurado siguiendo la plantilla maestra.
3.  **Nodo de Optimización y Revisión de Estilo:** El sistema revisa la legibilidad, sugiere asuntos potentes y verifica que todos los links funcionen correctamente.
4.  **Nodo de Dispatch y Segmentación:** El sistema envía la campaña al proveedor de email (API Beehiiv/ConvertKit) dirigiendo versiones específicas según segmentos.
5.  **Output:** Pieza editorial de alta calidad en el buzón de los suscriptores; reporte de aperturas y clics detallado; base de suscriptores fidelizada y en crecimiento.

---

## 7. Ejemplo Práctico: El Arquitecto 'Sostenible'
**Reto:** Marc es un arquitecto de bioconstrucción. Tenía 2000 emails de antiguos clientes y gente interesada, pero no les escribía nunca. Sentía que si les enviaba publicidad "les molestaría". No conseguía nuevos proyectos a través de su base de contactos.
**Acción v2.0:** Implementó Skill 283. Lanzó 'El Ladrillo de Barro', una newsletter quincenal donde analiza un material sostenible, critica un edificio famoso y recomienda un libro. No vende nada directamente, solo comparte su pasión y saber.
**Resultado:** Su Open Rate es del 62%. Marc se ha convertido en el referente de su nicho. Le han invitado a dar charlas en universidades y, lo más importante, recibe 2 o 3 solicitudes de presupuesto al mes de gente "que lee su carta" y confía plenamente en su criterio técnico.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
