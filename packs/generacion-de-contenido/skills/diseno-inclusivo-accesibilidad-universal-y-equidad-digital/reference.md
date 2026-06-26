# Referencia ampliada — Diseño Inclusivo, Accesibilidad Universal y Equidad Digital

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control de accesibilidad automatizada.*

1.  **Trigger:** El equipo de desarrollo sube una nueva página de "Checkout" al entorno de integración.
2.  **Nodo de Auditoría Axe Automática:** El sistema escanea el código buscando botones sin etiqueta `aria-label` o imágenes sin `alt`.
3.  **Nodo de Simulación de Visión IA:** El sistema genera capturas de la pantalla aplicando filtros de daltonismo (Protanopia, Deuteranopia) y borrosidad de visión.
4.  **Nodo de Alerta de Contraste Dinámico:** Si un componente cambia de color en base a datos y el contraste baja de 4.5:1, el sistema envía una alerta crítica.
5.  **Output:** Informe técnico de cumplimiento de accesibilidad con soluciones de código directas para los desarrolladores.

---

## 7. Ejemplo Práctico: App de Mensajería para Salud Pública
**Reto:** La App de citas médicas no permitía que las personas ciegas reservaran cita de forma autónoma porque el calendario no era accesible por teclado.
**Acción v2.0:** Se rediseñó el calendario usando un componente accesible certificado, se añadieron etiquetas de voz claras y se simplificó la carga cognitiva de los formularios.
**Resultado:** Se garantizó el derecho a la salud autónoma del 100% de la población; las quejas por inaccesibilidad desaparecieron y la plataforma fue premiada por su inclusividad.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
