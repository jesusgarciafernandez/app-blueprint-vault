# Referencia ampliada — Maquetación, Layout de Alta Densidad y Sistemas de Rejilla

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de adaptación de layout automatizada.*

1.  **Trigger:** El sistema detecta que el usuario está accediendo a la landing desde un dispositivo de resolución inusual (ej: Pantalla ultra-panorámica).
2.  **Nodo de Re-cálculo de Rejilla:** IA ajusta automáticamente los márgenes laterales para que la longitud de línea del texto siga siendo óptima (entre 45 y 75 caracteres).
3.  **Nodo de Re-ordenación Jerárquica:** El sistema prioriza los elementos de mayor conversión en la parte superior ('above the fold') según el nuevo espacio disponible.
4.  **Nodo de Verificación de Alineación:** Comprobación automática de que ningún elemento se sale del "contenedor maestro" definido por el sistema de rejilla.
5.  **Output:** Interfaz perfectamente maquetada y visualmente equilibrada entregada al usuario final sin intervención manual.

---

## 7. Ejemplo Práctico: Portal de Noticias Financieras
**Reto:** Su web era un caos de banners, noticias y gráficos que causaba rechazo inmediato al entrar.
**Acción v2.0:** Se aplicó una retícula modular estricta inspirada en periódicos suizos. Se aumentó el espacio en blanco y se jerarquizaron las noticias por tamaño de caja proporcional a su relevancia.
**Resultado:** La tasa de rebote bajó un 35% y los usuarios empezaron a navegar por 3 artículos más de media por sesión, gracias a la nueva claridad y orden visual.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
