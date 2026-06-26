# Referencia ampliada — Automatización Comercial Avanzada de SaaS (B2B SaaS Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de crecimiento escalable.*

1.  **Trigger:** Un usuario se registra en la plataforma o realiza una acción crítica de producto.
2.  **Nodo de Enriquecimiento de Datos:** El sistema consulta APIs externas (Clearbit/Apollo) para obtener el tamaño de empresa y sector del lead.
3.  **Nodo de Clasificación y Routing:** IA decide si el lead va a un flujo de "Self-Service" (Email automation) o se asigna a un "Account Ejecutivo" (Sugerencia de llamada).
4.  **Nodo de Acción de Engagement:** Disparo de la secuencia correspondiente y actualización del pipeline en el CRM en tiempo real.
5.  **Output:** Lead moviéndose por el embudo sin intervención manual; el sistema genera un reporte semanal de velocidad de ventas y cuellos de botella.

---

## 7. Ejemplo Práctico: SaaS de Gestión de Proyectos
**Reto:** El 70% de los usuarios que se registraban no volvían a entrar después de 2 días.
**Acción v2.0:** Se implementó una automatización que detectaba si el usuario no había creado su primer proyecto en las primeras 4 horas. Al detectar esto, enviaba un vídeo tutorial corto personalizado vía email y abría una tarea en el CRM para que el equipo de Customer Success enviara un mensaje de ayuda.
**Resultado:** La tasa de activación de usuarios subió un 40% y el paso de free-trial a pago se duplicó en 3 meses.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
