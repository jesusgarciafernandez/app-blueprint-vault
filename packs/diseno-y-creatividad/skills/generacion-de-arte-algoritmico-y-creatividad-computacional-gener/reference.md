# Referencia ampliada — Generación de Arte Algorítmico y Creatividad Computacional (Generative Art)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de creación de activos creativos.*

1.  **Trigger:** El usuario solicita una pieza de arte personalizada o se recibe un nuevo flujo de datos (Ej: Precio de Bitcoin).
2.  **Nodo de Traducción Creativa:** IA traduce el input en parámetros técnicos para el motor generativo (Ej: "Tristeza" -> Colores fríos, baja saturación, formas lentas).
3.  **Nodo de Motor Generativo (Server-side):** Ejecución del workflow en ComfyUI o script de Processing para generar la imagen/animación.
4.  **Nodo de Validación Estética:** El sistema compara la salida con un modelo de "Estética de Marca" para descartar errores técnicos (glitches no deseados).
5.  **Output:** Obra generada y entregada en alta resolución; el sistema guarda la semilla (Seed) para permitir ajustes futuros.

---

## 7. Ejemplo Práctico: Festival de Música Electrónica
**Reto:** Necesitaban visuales que reaccionaran al BPM y a la intensidad de la música de 10 DJs diferentes sin intervención manual durante 5 horas.
**Acción v2.0:** Se programó un sistema en Shaders (GLSL) que mutaba las formas y colores según las frecuencias de audio filtradas en tiempo real.
**Resultado:** Una experiencia visual única para cada set, donde la música y la luz se sentían como un único organismo vivo, aumentando la inmersión del público y reduciendo el equipo de VJs a una sola persona de supervisión.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
