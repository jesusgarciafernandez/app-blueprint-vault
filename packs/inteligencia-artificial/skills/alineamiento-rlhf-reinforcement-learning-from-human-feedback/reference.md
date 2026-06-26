# Referencia ampliada — Alineamiento RLHF (Reinforcement Learning from Human Feedback)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Creación del Modelo de Recompensa (Reward Modeling)
**Objetivo:** Enseñar a un modelo secundario a "pensar" como un humano evaluador.
1.  **Recolección de Rankings:** IA ayuda a generar múltiples respuestas para cada prompt y el humano las ordena de mejor a peor.
2.  **Entrenamiento del Juez Sintético:** El 'Reward Model' se entrena para predecir qué respuesta elegiría el humano, convirtiendo la preferencia en un valor escalar.

**Prompt Maestro de Alineamiento RLHF:**
```text
Actúa como un Senior Alignment Researcher y Experto en IA Responsable. Diseña el proceso de RLHF para el modelo [MODELO]. 
1. Rúbrica de Preferencia Human: Define los 3 criterios clave que los evaluadores usarán para puntuar (Ej: Veracidad, Tono servicial, Concisión) y redacta ejemplos de 'Pase' y 'Fallo'. 
2. Configuración del Modelo de Recompensa (RM): Propón la arquitectura del RM y diseña el proceso de validación para asegurar que el RM y los humanos están de acuerdo en al menos el 80% de los casos. 
3. Estrategia de Optimización (PPO): Establece los hiperparámetros de penalización 'KL-Divergence' para que el modelo no se aleje demasiado de su conocimiento base mientras aprende a ser más útil. 
4. Mitigación de 'Reward Hacking': Diseña 5 casos de prueba para detectar si el modelo ha aprendido a "engañar" al RM (Ej: dando respuestas cortas que suenan bien pero no dicen nada). 
5. Protocolo de Evaluación de Alineamiento: Define cómo usaremos un modelo superior (Ej: GPT-4o) para auditar el progreso del alineamiento de forma automatizada y objetiva.
```

### Fase 2: Ejecución del Bucle RL y Validación Conductual
... (Expansión técnica sobre el uso de la técnica de 'Preference Data Augmentation' para escalar el set de entrenamiento, la implementación de un proceso de 'Safe-RL' para evitar desviaciones peligrosas durante el entrenamiento y la monitorización de la 'Deriva de Capacidades' para asegurar que el modelo no pierde potencia en tareas técnicas mientras se vuelve más amable) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de mentoría sintética.*

1.  **Trigger:** Finalización del Fine-tuning Supervisado; el modelo conoce los datos pero puede ser grosero o inexacto.
2.  **Nodo de Generación y Comparación:** El sistema produce pares de respuestas y utiliza el 'Reward Model' pre-entrenado para asignar puntuaciones de "calidad humana".
3.  **Nodo de Actualización de Política (PPO Loop):** La red neuronal del LLM se ajusta paso a paso para maximizar la puntuación recibida del modelo de recompensa.
4.  **Nodo de Auditoría de Alineamiento Ético:** Un proceso verifica que el nuevo comportamiento no ha introducido sesgos ni debilidades de seguridad imprevistas.
5.  **Output:** Modelo alineado (RLHF-tuned) listo para interactuar con humanos; reporte de mejora en métricas de utilidad y seguridad generado.

---

## 7. Ejemplo Práctico: Asistente Senior 'HelpfulAI'
**Reto:** Su modelo de atención al cliente era técnicamente perfecto pero sonaba arrogante y a veces daba instrucciones peligrosas si se le presionaba (jailbreak).
**Acción v2.0:** Aplicaron RLHF (Skill 217). 50 expertos en atención al cliente clasificaron 10.000 respuestas. Entrenaron un modelo de recompensa y optimizaron con PPO.
**Resultado:** El modelo se volvió empático, servicial y capaz de rechazar peticiones dañinas con educación. La satisfacción del usuario subió de 3.2 a 4.8 estrellas en solo un mes.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
