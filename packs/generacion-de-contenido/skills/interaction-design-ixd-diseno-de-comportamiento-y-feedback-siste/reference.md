# Referencia ampliada — Interaction Design (IxD), Diseño de Comportamiento y Feedback Sistémico

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de validación de interacción automatizada.*

1.  **Trigger:** El diseñador crea un nuevo componente de "Deslizador de Precios" con una lógica de interacción compleja.
2.  **Nodo de Simulación de Usuario IA:** Un bot interactúa con el componente miles de veces probando velocidades, ángulos y presiones diferentes.
3.  **Nodo de Detección de 'Dead Ends':** El sistema identifica si hay algún estado donde el usuario se quede bloqueado sin saber cómo volver atrás.
4.  **Nodo de Verificación de Latencia Visual:** IA comprueba si la transición entre estados tarda más de 100ms (umbral de percepción de lentitud).
5.  **Output:** Informe de "Salud de la Interacción" con sugerencias para mejorar el Affordance o ajustar los tiempos de feedback visual.

---

## 7. Ejemplo Práctico: App de Edición de Video Móvil
**Reto:** Los usuarios se sentían frustrados porque mover clips en la línea de tiempo era impreciso y a menudo los borraban por error.
**Acción v2.0:** Se rediseñó la interacción. Al tocar un clip, el móvil da una vibración sutil (Feedback háptico). Al moverlo, los otros clips se apartan con suavidad (Física creíble). El borrado requiere un gesto de "lanzar fuera" con confirmación visual de 'papelera'.
**Resultado:** La precisión en la edición subió un 50% y los errores de borrado accidental bajaron a cero, convirtiendo una tarea estresante en una experiencia lúdica y potente.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
