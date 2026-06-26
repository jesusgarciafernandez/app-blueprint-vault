# Referencia ampliada — Diseño Responsivo, Interfaces Fluidas y Arquitectura Multi-resolución

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de verificación de layout automatizada.*

1.  **Trigger:** El desarrollador sube los cambios de estilo de la Home al entorno de Staging.
2.  **Nodo de Escaneo Multi-resolución:** IA genera capturas automáticas de la página en 50 tamaños de pantalla diferentes (del iPhone SE al Monitor 4K).
3.  **Nodo de Detección de Colisión:** El sistema identifica si algún texto se sale de su contenedor o si hay solapamiento de elementos en niveles intermedios.
4.  **Nodo de Auditoría de Pesos de Asset:** Verificación automática de que las imágenes se están cargando en el tamaño correcto para cada resolución detectada.
5.  **Output:** Reporte de errores de layout responsivo con indicación exacta de la línea de CSS que está causando el fallo.

---

## 7. Ejemplo Práctico: Periódico Digital Internacional
**Reto:** En tablets, los artículos se leían fatal porque la columna de texto era demasiado ancha, causando fatiga visual. En móviles, las imágenes tardaban 5 segundos en cargar.
**Acción v2.0:** Se implementó una tipografía fluida con `clamp()` y una rejilla responsiva que ajusta los márgenes dinámicamente según el ancho. Se activó el reescalado de imágenes del lado del servidor.
**Resultado:** El tiempo de lectura por sesión subió un 30% en tablets y la tasa de rebote en móviles bajó a la mitad gracias a la carga instantánea de los assets.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
