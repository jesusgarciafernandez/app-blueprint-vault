# Referencia ampliada — Evaluación de Calidad IA (AI Benchmarking & Model Quality)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de certificación continua.*

1.  **Trigger:** Cambio en el prompt, el modelo base o los datos del RAG detectado en el sistema de control de versiones.
2.  **Nodo de Lanzamiento de Suite de Pruebas:** El sistema clona el entorno y lanza el dataset de evaluación contra la nueva versión de la IA.
3.  **Nodo de Evaluación por IA Juez:** Un modelo supervisor califica cada respuesta basándose en las rúbricas predefinidas y calcula el score global.
4.  **Nodo de Análisis de Regresión:** El sistema compara los resultados con la versión anterior para asegurar que no ha habido una caída de calidad.
5.  **Output:** Informe de certificación "Apto/No Apto" para despliegue; equipo técnico informado sobre los fallos específicos para corrección.

---

## 7. Ejemplo Práctico: Fintech 'SafeBanker'
**Reto:** Su asistente de inversiones a veces recomendaba productos no autorizados o citaba leyes derogadas. No podían lanzarlo sin una garantía de seguridad total.
**Acción v2.0:** Implementaron una suite de 500 AI Evals automáticos. La IA "Juez" detectaba cualquier mención a productos fuera de catálogo o alucinaciones legales.
**Resultado:** Detectaron que el modelo alucinaba en el 12% de los casos complejos. Tras 3 iteraciones de re-prompting validadas por la suite, bajaron el error al 0.5% y obtuvieron la aprobación regulatoria para el lanzamiento.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
