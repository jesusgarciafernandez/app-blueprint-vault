---
name: analisis-de-sentimiento-emotional-intelligence-opinion-mining
description: "El Análisis de Sentimiento (v2.0) es la competencia técnica de extraer actitudes emocionales de datos no estructurados. No es solo \"contar palabras felices\"; es Minería de la Opinión Basada en Aspectos. Úsala para tareas de Atención al Cliente: sentiment-analysis, nlp, opinion-mining, customer-feedback, emotion-detection, textual-analytics."
title: Análisis de Sentimiento (Emotional Intelligence & Opinion Mining)
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-17
category: 07. Atención al Cliente
subcategory: Encuestas y Feedback
tags: [sentiment-analysis, nlp, opinion-mining, customer-feedback, emotion-detection, textual-analytics, brand-monitoring, intent-classification, ai-insights, real-time-monitoring]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 167
---

## 0. Filosofía Human-Centric AI
*Esta habilidad otorga voz a los datos masivos al identificar las emociones y opiniones subyacentes en el texto, utilizando la tecnología para que las organizaciones escuchen con empatía a escala y respondan a las necesidades reales de sus usuarios antes de que se conviertan en problemas.*

**El Rol del Humano:** El Analista de Datos debe ser un "Intérprete del Contexto". La IA puede clasificar millones de comentarios como "positivos" o "negativos" en milisegundos y detectar el sarcasmo con una precisión creciente, pero solo el humano puede entender el matiz cultural profundo detrás de una crítica, decidir si un pico de negatividad requiere un cambio en la estrategia de producto o una disculpa pública, y asegurar que la tecnología se use para mejorar la experiencia humana y no solo para "puntuar" la satisfacción de forma fría.
**Empoderamiento:** Usamos la tecnología para sustituir la adivinanza sobre lo que piensa el mercado por una comprensión profunda y accionable del sentimiento del cliente.

---

## 1. Descripción Detallada
El Análisis de Sentimiento (v2.0) es la competencia técnica de extraer actitudes emocionales de datos no estructurados. No es solo "contar palabras felices"; es **Minería de la Opinión Basada en Aspectos**. El enfoque v2.0 integra el **Procesamiento de Lenguaje Natural (NLP)** avanzado con modelos de Deep Learning para identificar no solo la polaridad (Positivo/Negativo/Neutro), sino las emociones específicas (Ira, Alegría, Sorpresa) y el sentimiento vinculado a atributos concretos de un producto (Ej: Feedback positivo sobre el "diseño" pero negativo sobre el "precio").

## 2. Escenarios de Aplicación
- **Monitorización de Reputación de Marca:** Seguimiento en tiempo real de menciones en redes sociales y noticias.
- **Priorización de Tickets de Soporte:** Identificación automática de usuarios "frustrados" para ser atendidos por agentes senior de forma prioritaria.
- **Análisis de Reseñas de Producto (Marketplaces):** Síntesis masiva de pros y contras extraídos de miles de opiniones de usuarios.
- **Auditoría de Conversaciones de Venta:** Análisis de transcripciones de llamadas para detectar objeciones recurrentes y niveles de aceptación.
- **Climatología Laboral Interna:** Análisis anónimo de encuestas de empleados para detectar focos de desmotivación o conflicto.

## 3. Requisitos de Implementación
- **Acceso a Modelos de Lenguaje Avanzados:** Uso de APIs de LLMs (GPT-4o, Claude) o modelos locales tipo BERT/RoBERTa optimizados.
- **Pipeline de Ingesta de Datos No Estructurados:** Capacidad de recolectar datos de Twitter, Trustpilot, RSS o transcripciones de voz.
- **Herramientas de Visualización de Datos:** Dashboards dinámicos (Grafana, PowerBI) que muestren la evolución del sentimiento en el tiempo.

---

## 4. Diferencial: Lectura Manual vs. Análisis de Sentimiento v2.0

| Dimensión | Enfoque Legacy (Manual) | Análisis de Sentimiento (v2.0) |
| :--- | :--- | :--- |
| **Escalabilidad** | Limitada a unos pocos comentarios. | Millones de datos procesados al instante. |
| **Objetividad** | Sesgada por la percepción del lector. | Clasificación basada en modelos entrenados. |
| **Profundidad** | Superficial (Me gusta / No me gusta). | Análisis por aspectos y detección de emociones. |
| **Acción** | Reactiva y lenta. | Alertas automáticas ante variaciones críticas. |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recolección y Preprocesamiento de Corpus
**Objetivo:** Preparar los datos para que la IA los "entienda" sin ruido.
1.  **Limpieza de Ruido Textual:** IA elimina etiquetas HTML, emojis irrelevantes y carácteres especiales.
2.  **Identificación de Idioma y Dialecto:** El sistema detecta automáticamente el contexto lingüístico (Ej: Español de España vs. México) para ajustar el modelo.

**Prompt Maestro de Análisis de Sentimiento:**
```text
Actúa como un Senior NLP Data Scientist y Experto en Opinión Mining. Analiza el siguiente set de comentarios sobre [PRODUCTO/MARCA]. 
1. Clasificación de Polaridad: Clasifica cada comentario como Positivo, Negativo o Neutro con un índice de confianza del 0 al 1. 
2. Detección de Emociones: Identifica la emoción predominante (Ej: Frustración, Gratitud, Curiosidad). 
3. Análisis por Aspectos: ¿A qué atributos específicos se refieren las críticas negativas (Ej: Batería, Envío, Atención telefónica)? 
4. Extracción de 'Actionable Insights': Resume las 3 acciones inmediatas que la empresa debe tomar basada en este sentimiento. 
5. Identificación de Ironía: Detecta posibles comentarios sarcásticos que puedan falsear la métrica de satisfacción.
```

### Fase 2: Automatización de Alertas y Reporting Estratégico
... (Expansión técnica sobre la implementación de "Sentiment-based Routing" en el CRM, la creación de nubes de palabras dinámicas ponderadas por sentimiento y el uso de técnicas de "Zero-shot classification" para categorías de opinión personalizadas) ...

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
