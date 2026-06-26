# Referencia ampliada — Clasificación Inteligente de Datos (AI Classification & Taxonomy Management)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Diseño de la Taxonomía y Selección de Modelo
**Objetivo:** Definir las reglas del juego de organización.
1.  **Auditoría de Categorías:** IA ayuda a proponer una lista de etiquetas (Taxonomía) basada en una muestra representativa de los datos reales.
2.  **Definición de 'Ground Truth':** Creación de un set de 100 ejemplos clasificados por un experto para validar la precisión de la IA.

**Prompt Maestro de Clasificación de Datos:**
```text
Actúa como un Senior Metadata Architect y Experto en Clasificación de Datos. Diseña el sistema de organización para el set: [DESCRIPCIÓN_DATOS]. 
1. Estructura de Taxonomía: Genera un árbol jerárquico de 2 niveles (Categoría Core -> Subcategoría) para clasificar la información de forma unívoca. 
2. Lógica de Puntos de Decisión: Redacta los criterios de distinción (Ej: ¿Cuándo algo es 'Ventas' y no 'Marketing'?) para alimentar al modelo de IA. 
3. Detección de Sensibilidad: Define qué patrones o palabras clave activarán la etiqueta 'Confidencial/PII' (Ej: Formatos de DNI, Tarjetas, Emails). 
4. Formateo de Salida: Configura la IA para que devuelva un JSON estructurado con (A) Label, (B) Confidence Score (0-1) y (C) Rationale (por qué lo clasificó así). 
5. Test de Ambigüedad: Identifica 5 casos 'frontera' y define la regla de desempate automática que debe aplicar el sistema.
```

### Fase 2: Ejecución, Validación de Confianza y Auditoría
... (Expansión técnica sobre el uso de la técnica de 'Few-shot Classification' para dar ejemplos al modelo, la implementación de un proceso de 'Confianza Mínima' donde las etiquetas con score < 0.7 se envían a revisión humana, y la monitorización de la 'Deriva de Concepto' para ajustar la taxonomía si los nuevos datos cambian de naturaleza con el tiempo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de organización automática.*

1.  **Trigger:** Entrada de un nuevo activo de información (Archivo/Email/Fila de base de datos) al sistema monitorizado.
2.  **Nodo de Extracción de Texto/Contexto:** IA detecta el idioma, el formato y extrae el cuerpo principal de información.
3.  **Nodo de Clasificación Multivariante:** El modelo aplica la taxonomía y asigna etiquetas temáticas, de sentimiento y de nivel de riesgo en paralelo.
4.  **Nodo de Acción según Etiqueta:** El sistema toma decisiones (Ej: "Mover a carpeta de Seguridad", "Notificar a Finanzas") basándose en la clasificación.
5.  **Output:** Dato categorizado y almacenado correctamente; registro de auditoría actualizado con el motivo de la clasificación.

---

## 7. Ejemplo Práctico: Multinacional 'LogisTag'
**Reto:** Recibían 50.000 emails de proveedores al mes en 10 idiomas. No sabían cuáles eran facturas, cuáles quejas y cuáles ofertas sin abrirlos uno a uno.
**Acción v2.0:** Implementaron Clasificación de Datos (Skill 206). La IA clasificó el 100% de los emails en tiempo real, asignando etiquetas de "Tipo de Trámite" y "Prioridad".
**Resultado:** El tiempo de respuesta a quejas críticas bajó de 48 horas a 5 minutos. Las facturas se movieron automáticamente a contabilidad sin pasar por la bandeja de entrada de los gestores, ahorrando 1.200 horas/hombre mensuales.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
