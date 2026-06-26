# Referencia ampliada — Visualización de Datos Avanzada (Custom BI & Interactive Data Art)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de renderizado dinámico.*

1.  **Trigger:** Cambio en el dataset origen o interacción del usuario en la interfaz.
2.  **Nodo de Pre-procesado Gráfico por IA:** El sistema calcula los límites de las escalas (Domains & Ranges) y filtra los datos a mostrar.
3.  **Nodo de Generación de Geometría:** IA genera el código SVG o las llamadas a Canvas necesarias para representar los datos.
4.  **Nodo de Gestión de Eventos:** El sistema escucha las interacciones del usuario y actualiza los gráficos vinculados en milisegundos.
5.  **Output:** Visualización interactiva y fluida; el usuario puede "tocar" los datos y obtener respuestas inmediatas y visuales.

---

## 7. Ejemplo Práctico: Multinacional 'LogisticsGlobal'
**Reto:** No conseguían ver dónde se perdían los paquetes en su red de 500 almacenes. El mapa de calor estándar de su BI era "una mancha roja ilegible".
**Acción v2.0:** Desarrollaron una visualización de grafos animada con D3.js. La IA trazo las rutas reales y detectó mediante el grosor de las líneas los tramos de congestión.
**Resultado:** Identificaron que el problema no eran los almacenes, sino 3 rutas de transporte específicas Saturadas. Al ver la red "viva", el equipo cambió el flujo de carga y los retrasos bajaron un 30% en un mes.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
