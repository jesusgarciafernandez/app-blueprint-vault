# Referencia ampliada — Visión por Computadora (Computer Vision & Visual Intelligence)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de reacción visual.*

1.  **Trigger:** Recepción de un frame de imagen a través de una API, cámara local o carga de archivo.
2.  **Nodo de Normalización Visual:** El sistema limpia la imagen y destaca las características relevantes (ej: aumentando el contraste en zonas oscuras).
3.  **Nodo de Inferencia de Inteligencia Visual:** La IA procesa la imagen identificando objetos, texto o patrones específicos definidos.
4.  **Nodo de Lógica de Negocio Visual:** IA evalúa el resultado (ej: "¿El número de personas supera el aforo permitido?") y genera una decisión.
5.  **Output:** Metadatos de la imagen y alertas enviadas a sistemas externos; imagen original con anotaciones guardada para auditoría humana.

---

## 7. Ejemplo Práctico: Logística 'SmartWarehouse'
**Reto:** Un almacén perdía un 5% de sus envíos porque las etiquetas se pegaban torcidas o eran ilegibles para los escáneres láser tradicionales.
**Acción v2.0:** Implementaron Visión por Computadora (Skill 230). Cámaras de alta velocidad capturan cada paquete; una IA (YOLO + OCR) detecta la etiqueta y lee la dirección independientemente del ángulo.
**Resultado:** La tasa de error bajó al 0.01%. El sistema ahora detecta incluso paquetes dañados antes de que salgan del almacén, enviando una alerta automática al equipo de embalaje.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
