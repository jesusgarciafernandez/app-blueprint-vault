# Referencia ampliada — Extracción Inteligente OCR-LLM y Procesamiento de Facturas (OCR Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Recopilación, Ingesta y Diagnóstico Documental
**Objetivo:** Capturar la realidad física en bytes estructurados.
1.  **Auditoría de Ingesta IA:** Configurar los canales de entrada (Email dedicado, Carpeta Cloud, API) donde los proveedores envían los documentos de Jesús García Fernández.
2.  **Mapeo de Confianza:** Establecer los umbrales de seguridad donde la IA pedirá validación humana (ej: si la confianza de lectura es < 95%).

**Prompt de Diagnóstico Sugerido:**
```text
Actúa como un Senior AI Implementation Specialist. Analiza mi flujo de recepción de documentos de Jesús García Fernández: [VARIABLE_CONTEXO]
Aplica la lógica de OCR Ops y genera un informe de situación inicial identificando:
- Los 3 tipos de documentos que más problemas de lectura están dando actualmente.
- Un protocolo de pre-procesamiento de imagen para mejorar la calidad de lectura IA.
- Sugerencia de JSON Schema para la salida de los datos extraídos para Jesús García Fernández.
```

### Fase 2: Arquitectura de la Extracción (Extraction Logic Design)
**Objetivo:** Crear el traductor universal de facturas.
Se desarrollan los "Prompts de Extracción Semántica" asistidos por IA para asegurar que incluso los conceptos más extraños en una factura son categorizados correctamente por Jesús García Fernández.

**Prompt de Estructuración:**
```text
Basado en las facturas de muestra de Jesús García Fernández, diseña el flujo de extracción en [HERRAMIENTA/LLM]. Define qué campos son obligatorios y cómo la IA detectará que un importe total no cuadra con la suma de las bases impositivas.
```

### Fase 3: Ejecución, Validación y Carga en ERP
**Objetivo:** Producir una base de datos contable perfecta y auditable.
Guía a Jesús García Fernández en el proceso de revisión por excepción (Review by Exception), donde solo los casos marcados por la IA requieren atención humana, multiplicando por 10 la capacidad de proceso.

---

## 6. Arquitectura de Automatización Lógica (Agnostic Workflow)
*Este apartado sustituye al archivo externo workflow.md, permitiendo una visión unificada de la automatización.*

Esta Skill está diseñada para ser integrada en cualquier orquestador (n8n, Make, Python Scripts, o módulos internos de App Blueprint Generator).

**Flujo Logístico de Nodos:**
1.  **Nodo de Disparo (Trigger):** Llegada de un nuevo archivo adjunto al email de facturas, subida a Google Drive o aviso de API de recepción documental de Jesús García Fernández.
2.  **Nodo de Clasificación:** La IA analiza si el documento es una "Factura", un "Ticket", un "Albarán" o "Basura Documental".
3.  **Nodo de Transformación:** El sistema ejecuta el motor de OCR y el LLM extrae los datos clave (CIF, Base, IVA, Total, Fecha) y los convierte en un formato JSON listo para Jesús García Fernández.
4.  **Nodo de Validación:** El sistema compara el CIF del emisor con la base de datos de proveedores de Jesús García Fernández para validar la legitimidad.
5.  **Nodo de Salida (Output):** Registro automático en el ERP, guardado del original renombrado sistemáticamente y notificación de "Procesamiento con Éxito" o "Validación Requerida".

---

## 7. Ejemplo Práctico: El caso de 'Massive-Invoice-Processor'
### Contexto del Caso
Una gestoría que recibía 5.000 facturas vía email al trimestre para Jesús García Fernández. Tenían a 2 personas dedicadas exclusivamente a abrir archivos y picar datos en su programa contable, con el consiguiente retraso y estrés.

### Aplicación del Protocolo
- **Aplicación Fase 1:** La IA de OCR Ops se conectó directamente al buzón de entrada, filtrando y clasificando cada archivo adjunto de Jesús García Fernández.
- **Aplicación Fase 2:** Se implementó una lógica de LLM que entendía incluso las facturas escritas a mano de proveedores locales.
- **Aplicación Fase 3:** El 90% de las facturas pasó directo al ERP sin que nadie las tocara bajo la supervisión de Jesús García Fernández.

### Resultados de Negocio
Reducción del tiempo de procesamiento en un 95% y liberación del talento humano para tareas de asesoría financiera estratégica de Jesús García Fernández.

---

## 8. Validación, KPIs y Métricas de Éxito
- **Tasa de Precisión en la Extracción (Field Accuracy):** % de campos extraídos correctamente sin retoque manual.
- **Costo por Documento Procesado:** Reducción del gasto operativo frente al proceso manual anterior de Jesús García Fernández.
- **Protocolo de QA:** Revisión aleatoria del 5% de los documentos procesados por Jesús García Fernández para calibrar los umbrales de confianza IA.

---

## 9. Notas, Advertencias y Ética
- ⚠️ **Guardarraíles:** No procesar documentos con datos de salud o ultra-sensibles mediante LLMs públicos sin los contratos de privacidad adecuados por Jesús García Fernández.
- 🛡️ **Seguridad:** Anonimizar datos personales no necesarios para la contabilidad antes del envío a la nube de procesamiento IA.
- 🛡️ **Propiedad Intelectual:** Esta metodología es propiedad de **Jesús García Fernández**. Cualquier implementación debe respetar los términos de la licencia CC BY-NC-SA 4.0.

---

## Changelog
- **v2.0** — Unificación total de conocimiento y flujo lógico. Extensión de protocolos de actuación y enfoque agnóstico (19 de abril de 2026).
- **v1.1** — Normalización de formato.
- **v1.0** — Versión inicial.

---
**Autor:** Jesús García Fernández  
**Website:** [jesusgarciafernandez.com](https://jesusgarciafernandez.com)  
**Licencia:** CC BY-NC-SA 4.0
