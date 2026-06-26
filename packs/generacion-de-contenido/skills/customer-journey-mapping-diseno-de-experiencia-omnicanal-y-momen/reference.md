# Referencia ampliada — Customer Journey Mapping, Diseño de Experiencia Omnicanal y Momentos de la Verdad

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de monitorización del Journey automatizada.*

1.  **Trigger:** Un usuario detiene su proceso de registro en la pantalla de "subir documento de identidad" durante más de 60 segundos.
2.  **Nodo de Identificación de Fricción:** IA detecta que el Journey se ha roto en el touchpoint de 'Validación' por un sentimiento de "confusión o pereza".
3.  **Nodo de Intervención Contextual:** El sistema activa un chat de ayuda automático o envía un trigger a soporte para una llamada proactiva.
4.  **Nodo de Registro en el Mapa Agregado:** El incidente se guarda automáticamente en la base de datos de CX para actualizar el 'Mapa de Calor de Fricción' del mes.
5.  **Output:** Informe mensual dinámico que indica qué fases del Journey están perdiendo más usuarios y propone cambios estructurales.

---

## 7. Ejemplo Práctico: Banca Digital para Jóvenes
**Reto:** Los usuarios empezaban el alta en la App pero solo el 10% la terminaba. No se sabía dónde estaba el problema.
**Acción v2.0:** Se mapeó el Journey completo y se descubrió que el punto de dolor era la espera de 24h para la validación del DNI. El nivel emocional caía a "aburrimiento/olvido".
**Resultado:** Se rediseñó el proceso para que la validación fuera en tiempo real (Backstage upgrade). La tasa de conversión de altas subió al 45% en un solo mes.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
