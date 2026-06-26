# Referencia ampliada — AI Sparring (Cognitive Reasoning & Expert Troubleshooting)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de desbloqueo cognitivo.*

1.  **Trigger:** Identificación de un punto de bloqueo o duda que requiere un análisis superior a una búsqueda simple.
2.  **Nodo de Extracción de Contexto:** El sistema solicita al usuario el entorno del problema (código, documentos, objetivos) y los intentos previos.
3.  **Nodo de Razonamiento Iterativo IA:** La IA genera una primera hipótesis y lanza preguntas para refinar la dirección del pensamiento.
4.  **Nodo de Propuesta de Solución y Crítica:** El sistema entrega la solución acompañada de una crítica de sus propios puntos débiles.
5.  **Output:** Solución implementada y entendida por el humano; base de conocimientos actualizada con la nueva solución para evitar futuras dudas.

---

## 7. Ejemplo Práctico: Depuración de Código 'GhostBug'
**Reto:** Un desarrollador llevaba 4 horas atascado con un error de memoria en una aplicación compleja que ni Google ni los foros explicaban.
**Acción v2.0:** Usó el Sparring de IA (Skill 223). En lugar de pedir el código correcto, pidió a la IA que actuara como un "Analista de Trazas". La IA le hizo preguntas sobre la concurrencia de hilos que el desarrollador no había considerado.
**Resultado:** En 10 minutos, el desarrollador comprendió que el fallo estaba en una condición de carrera extraña. La IA no solo le dio el parche, sino que le enseñó a detectar ese patrón en el futuro, elevando su nivel como programador.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
