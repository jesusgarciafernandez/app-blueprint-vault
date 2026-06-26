# Referencia ampliada — Explicabilidad de la IA (XAI & Transparent AI Reasoning)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Visibilidad y Diseño de Justificaciones
**Objetivo:** Definir qué partes de la decisión deben ser explicables y para quién.
1.  **Identificación de Stakeholders:** IA ayuda a definir si la explicación es para un técnico (Python logs) o para un cliente (narrativa sencilla).
2.  **Selección de Método XAI:** Determinación de si usaremos una importancia global del modelo o una explicación local (para una sola decisión concreta).

**Prompt Maestro de Explicabilidad (XAI Strategy):**
```text
Actúa como un Senior XAI Engineer y Auditor de Transparencia Algorítmica. Diseña el marco de explicabilidad para el sistema [NOMBRE_MODELO/TAREA]. 
1. Análisis de Importancia: Identifica las 3 variables de entrada que el sistema considera críticas para [DATO_SALIDA] y explica su relación lógica. 
2. Diseño de la Narrativa de Justificación: Redacta un prompt de 'Explicador' que traduzca datos numéricos en un párrafo comprensible para un usuario no técnico. 
3. Visualización de Atención: Diseña el mapa de calor visual (Heatmap) que mostrará en qué parte de la información se enfocó el modelo para dar la respuesta. 
4. Detección de 'Causas de Error': Propón un método para alertar si el modelo está tomando decisiones basadas en ruido o variables no deseadas. 
5. Protocolo de Transparencia: Genera el formato de 'Ficha de Decisión' que se adjuntará a cada output para cumplir con el derecho a la explicación.
```

### Fase 2: Implementación, Validación de Fidelidad y Reporte
... (Expansión técnica sobre el uso de la técnica de 'Feature Attribution' para cuantificar el impacto de cada palabra en un prompt, la implementación de tests de fidelidad (Faithfulness) para asegurar que la explicación corresponde realmente a la lógica interna del modelo, y la creación de un sistema de transparencia proactiva que alerte si la interpretabilidad del sistema cae por debajo de un umbral aceptable) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de transparencia continua.*

1.  **Trigger:** Decisión tomada por un modelo de IA en un proceso crítico de negocio o usuario.
2.  **Nodo de Extracción de Pesos/Atención:** El sistema recupera la importancia de las características o los pesos de atención de la red neuronal para esa decisión específica.
3.  **Nodo de Síntesis Narrativa XAI:** IA traduce los valores matemáticos de importancia en una justificación textual alineada con la rúbrica de explicabilidad.
4.  **Nodo de Verificación de Alineación Ética:** Un proceso monitoriza que la explicación no revele datos privados ni intente justificar sesgos prohibidos.
5.  **Output:** Decisión final acompañada de su justificación comprensible; log de transparencia almacenado para futuras auditorías o reclamaciones del usuario.

---

## 7. Ejemplo Práctico: Aseguradora 'ClearProtect'
**Reto:** Su IA denegaba pólizas de vida a personas sanas sin razón aparente. El equipo técnico no sabía qué estaba fallando y los clientes estaban indignados.
**Acción v2.0:** Implementaron XAI (Skill 207). El sistema reveló que la IA estaba dando un peso excesivo a una variable secundaria (el modelo de smartphone del cliente) que actuaba como proxy de estatus económico, no de salud.
**Resultado:** Identificaron y eliminaron el sesgo en 24 horas. Ahora, cada denegación incluye una carta personalizada que explica detalladamente (y éticamente) los factores de salud considerados, aumentando la confianza del cliente un 40%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
