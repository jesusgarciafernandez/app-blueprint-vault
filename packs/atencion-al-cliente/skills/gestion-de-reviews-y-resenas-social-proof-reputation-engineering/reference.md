# Referencia ampliada — Gestión de Reviews y Reseñas (Social Proof & Reputation Engineering)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de gestión de prueba social.*

1.  **Trigger:** Entrega de producto confirmada por el transportista o cierre de ticket de soporte con éxito.
2.  **Nodo de Envío de Solicitud:** El sistema manda un mensaje personalizado invitando a valorar la experiencia.
3.  **Nodo de Recepción y Análisis:** Al publicarse la reseña, IA analiza el contenido, clasifica el sentimiento y propone un borrador de respuesta.
4.  **Nodo de Notificación Crítica:** Si la reseña es < 3 estrellas, se notifica al gerente local por Slack para intervención inmediata.
5.  **Output:** Perfil público activo y confiable; los potenciales clientes ven una marca que escucha y resuelve, aumentando la conversión final.

---

## 7. Ejemplo Práctico: Clínica Dental 'Sonrisa Real'
**Reto:** Tenían 4.2 estrellas en Google pero solo 10 reseñas. Mucha gente llamaba diciendo que "no tenían suficientes opiniones".
**Acción v2.0:** Instalaron un QR en recepción que enviaba un mensaje de WhatsApp agradeciendo la visita y pidiendo opinión 1 hora después de la cita.
**Resultado:** En 2 meses pasaron de 10 a 85 reseñas. Su nota subió a 4.8. Las llamadas de potenciales clientes desde Google Maps aumentaron un 60%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
