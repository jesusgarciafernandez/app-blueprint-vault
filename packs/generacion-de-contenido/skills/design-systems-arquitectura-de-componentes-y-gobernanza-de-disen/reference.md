# Referencia ampliada — Design Systems, Arquitectura de Componentes y Gobernanza de Diseño

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de sincronización de diseño y código.*

1.  **Trigger:** El Lead Designer cambia el radio de esquina de los botones de 4px a 8px en el archivo maestro de Figma.
2.  **Nodo de Traducción a JSON:** IA detecta el cambio y actualiza automáticamente el archivo de Style Dictionary de los Design Tokens.
3.  **Nodo de Despliegue Automático:** Las variables se envían al repositorio de GitHub y activan una compilación de las librerías CSS/Swift/Kotlin.
4.  **Nodo de Verificación de Regresión:** Un bot saca capturas de las pantallas principales de la App y confirma que el cambio es consistente en todos los dispositivos.
5.  **Output:** Nueva versión del sistema desplegada en segundos sin que ningún desarrollador haya tenido que escribir una sola línea de CSS.

---

## 7. Ejemplo Práctico: Multinacional de Seguros
**Reto:** Tenían 40 webs diferentes y cada una usaba un botón de "Pagar" distinto. Cualquier cambio de marca costaba 6 meses de trabajo.
**Acción v2.0:** Se creó un Design System con tokens semánticos y una librería de componentes compartidos. Se implementó una gobernanza de "Contribución Abierta".
**Resultado:** Se redujo el tiempo de diseño de nuevas pantallas en un 70% y el primer rebranding de color se completó en solo 1 semana en lugar de medio año.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
