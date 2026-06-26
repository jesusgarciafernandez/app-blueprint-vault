# Referencia ampliada — Excelencia en Revisión de Código y Mentoría (Engineering Craftsmanship)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de PR y Preparación de la Sesión de Mentoría
**Objetivo:** Identificar los puntos de palanca para elevar la calidad del código.
1.  **Revisión Automática Previa:** IA ayuda a correr análisis estáticos para limpiar la PR de errores de formato o sintaxis triviales.
2.  **Análisis de Impacto Arquitectónico:** Evaluación de cómo los cambios afectan a otros módulos y a la deuda técnica global.

**Prompt Maestro de Mentoría Técnica (Code Craftsmanship):**
```text
Actúa como un CTO y Principal Engineer con alta dosis de empatía. Revisa la lógica del código en [REPOSITORIO/DIFFERENTIAL/PR]. 
1. Diagnóstico de Calidad: Identifica las 3 zonas de código que tienen mayor riesgo de convertirse en deuda técnica o son difíciles de leer. 
2. Guía Socrática de Mentoría: Redacta 3 comentarios para la PR que no den la solución directamente, sino que pregunten al desarrollador por alternativas de diseño (Ej: ¿Qué pasaría si necesitamos añadir un tercer tipo de usuario aquí?). 
3. Alineamiento con SOLID: Indica dónde se están violando principios de arquitectura limpia y propón un patrón de diseño (Ej: Factory, Strategy) que simplifique la implementación. 
4. Check de Seguridad y Performance: Detecta posibles cuellos de botella o vulnerabilidades (Ej: N+1 queries, Inyecciones) que la IA de linteo haya pasado por alto. 
5. Resumen Positivo y Pasos Siguientes: Redacta un mensaje de cierre que celebre los aciertos del código y resuma las áreas de mejora clave para la aprobación final.
```

### Fase 2: Ejecución de Revisión Interactiva y Cierre
... (Expansión técnica sobre el uso de la técnica de 'Approval with comments' donde se aprueba bajo ciertas condiciones menores, la implementación de un proceso de 'Summary of Learning' donde el mentor y el mentoreado resumen qué han aprendido en esa revisión, y la monitorización del 'Time-to-Review' para asegurar que la calidad no bloquee la velocidad del equipo) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de transferencia de maestría.*

1.  **Trigger:** Creación de una 'Pull Request' o solicitud de revisión de código por parte de un desarrollador.
2.  **Nodo de Pre-Auditoría con IA:** Un agente analiza el código buscando antipatrones conocidos, falta de tests unitarios y problemas de estilo.
3.  **Nodo de Resumen Estratégico para el Mentor:** El sistema presenta al mentor humano los cambios clave de lógica y sugiere los puntos donde la mentoría sería más valiosa.
4.  **Nodo de Interacción Humana (Mentoría):** El mentor añade comentarios descriptivos y educativos; se inicia un diálogo técnico en el hilo de la revisión.
5.  **Output:** Código aprobado y verificado; aprendizaje consolidado en el desarrollador; registro de la sesión guardado para el historial de crecimiento del equipo.

---

## 7. Ejemplo Práctico: Startup 'ScaleOps'
**Reto:** El equipo creció de 3 a 15 ingenieros en 6 meses. La calidad del código cayó en picado, cada uno programaba a su estilo y los despliegues empezaron a ser una pesadilla de errores inesperados.
**Acción v2.0:** Implementaron Excelencia en Revisión de Código (Skill 232). Cada PR requería dos revisiones obligatorias, una de las cuales debía tener un enfoque educativo. Usaron una IA de linteo para el formato y un 'Reviewer de Turno' experto para la lógica.
**Resultado:** Los errores en producción bajaron un 70% en el primer trimestre. El sentimiento de pertenencia al equipo subió, y los desarrolladores junior reportaron que aprendían más en una PR de ScaleOps que en un curso entero de programación.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
