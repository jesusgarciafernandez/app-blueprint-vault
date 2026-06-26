# Referencia ampliada — Prototipado Rápido (Figma), Lógica Condicional y Simulaciones de Alta Fidelidad

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de creación de prototipos automatizada.*

1.  **Trigger:** El diseñador termina de definir el User Flow en un diagrama (Sitemap/Miro).
2.  **Nodo de Traducción a Figma IA:** El sistema genera automáticamente el esquema de pantallas y conecta los botones principales basándose en el diagrama de flujo.
3.  **Nodo de Inyección de Librería de Estilos:** IA aplica automáticamente los componentes maestros (botones, menús) del Design System a los bloques placeholder.
4.  **Nodo de Verificación de Enlaces Rotos:** Un bot recorre el prototipo buscando botones sin destino o transiciones incoherentes antes de compartir el enlace.
5.  **Output:** Enlace de prototipo funcional funcional y listo para la primera fase de revisión con el cliente.

---

## 7. Ejemplo Práctico: App de Delivery de Comida
**Reto:** El cliente no entendía cómo funcionaba el "seguimiento en el mapa" mirando imágenes estáticas.
**Acción v2.0:** Se creó un prototipo avanzado con Smart Animate donde el ciclista se mueve realmente por el mapa tras 2 segundos. Se usaron variables para que el usuario pudiera "añadir hamburguesas" y ver cómo subía el precio del carrito en tiempo real.
**Resultado:** El cliente quedó impresionado ("¡Parece real!"). Se detectó que el botón de 'Pagar' era confuso en pantallas pequeñas y se corrigió antes de programar, evitando semanas de retrabajo técnico.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
