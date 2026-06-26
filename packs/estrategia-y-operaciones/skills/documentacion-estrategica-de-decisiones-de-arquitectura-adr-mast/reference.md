# Referencia ampliada — Documentación Estratégica de Decisiones de Arquitectura (ADR Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de gestión de conocimiento.*

1.  **Trigger:** Se detecta un cambio mayor en la estructura del proyecto o un debate técnico prolongado en las herramientas de comunicación.
2.  **Nodo de Extracción de Intención:** IA analiza la discusión y propone un borrador inicial de ADR capturando los puntos clave de cada participante.
3.  **Nodo de Validación contra Estándares:** El sistema comprueba si la decisión propuesta rompe algún 'Guardrail' de arquitectura previamente definido en otros ADRs.
4.  **Nodo de Distribución de Revisión:** Envía el borrador a los 'Stakeholders' técnicos para su validación final y firma digital (Acceptance).
5.  **Output:** ADR registrado en el repositorio; la memoria técnica de la empresa se actualiza y el riesgo de "Amnistía de Arquitectura" se reduce a cero.

---

## 7. Ejemplo Práctico: Startup de Streaming de Vídeo
**Reto:** Habían decidido usar WebRTC para baja latencia, pero 6 meses después la mayoría de usuarios sufrían cortes. Nadie recordaba por qué no usaron HLS desde el principio.
**Acción v2.0:** Se consultó el ADR #12. Allí se explicaba que en ese momento el 90% de los usuarios eran B2B con redes locales potentes. Al pasar a B2C, el contexto cambió. Gracias al ADR, pudieron pivotar a HLS de forma rápida sabiendo exactamente qué partes del sistema se verían afectadas.
**Resultado:** La estabilidad del servicio subió al 99.9% y el equipo de ingeniería evitó culpas innecesarias al entender que la decisión original fue correcta para el contexto de aquel momento.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
