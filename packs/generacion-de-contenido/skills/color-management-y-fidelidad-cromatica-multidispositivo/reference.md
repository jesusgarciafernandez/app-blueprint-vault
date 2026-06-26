# Referencia ampliada — Color Management y Fidelidad Cromática Multidispositivo

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de integridad cromática.*

1.  **Trigger:** El sistema recibe una imagen para ser publicada en la web.
2.  **Nodo de Inspección de Metadatos:** IA verifica si el archivo tiene un perfil de color incrustado.
3.  **Nodo de Conversión Inteligente:** Si el perfil es ProPhoto o Adobe RGB, el sistema realiza una conversión a sRGB con compensación de contraste para evitar que el color se vea "lavado" en navegadores estándar.
4.  **Nodo de Validación de Marca:** El sistema escanea la imagen buscando los colores corporativos y verifica que la desviación (Delta E) sea inferior a 2.0.
5.  **Output:** Activo visual optimizado y cromáticamente correcto entregado al gestor de contenidos.

---

## 7. Ejemplo Práctico: Marca de Pintura para Automóviles
**Reto:** Los clientes se quejaban de que el color de la web no se parecía en nada al color real de la pintura recibida.
**Acción v2.0:** Se implementó un flujo de gestión de color riguroso desde la fotografía de las muestras hasta el uso de perfiles ICC específicos para pantallas móviles dominantes (iPhone/Pixel).
**Resultado:** Las reclamaciones por falta de coincidencia de color bajaron un 80% y la satisfacción del cliente aumentó significativamente al recibir exactamente lo que esperaba ver.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
