# Referencia ampliada — Pagos y Suscripciones (Stripe Master Performance)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de orquestación de ingresos.*

1.  **Trigger:** El cliente hace clic en "Suscribirse" y completa el flujo de pago.
2.  **Nodo de Validación Post-Pago (Webhook):** El sistema recibe la señal 'checkout.session.completed' y verifica la autenticidad de la firma.
3.  **Nodo de Aprovisionamiento de Servicio:** El sistema activa automáticamente los permisos de la cuenta del usuario en la base de datos local y el CRM.
4.  **Nodo de Facturación y Bienvenida:** Envío automático de la factura legal y correo de "Éxito" con los primeros pasos (Skill 159).
5.  **Output:** Cliente activo y dinero en tránsito; reporte de ingresos actualizado sin haber movido un solo dedo.

---

## 7. Ejemplo Práctico: Plataforma de Cursos 'Creative Lab'
**Reto:** El dueño perdía 2 días al mes emitiendo facturas a mano y comprobando quién había pagado por transferencia. Muchos alumnos accedían sin haber pagado.
**Action v2.0:** Se integró Stripe. Los alumnos pagan con tarjeta o Apple Pay. El acceso al curso se desbloquea al instante. Si un pago mensual falla, el sistema les quita el acceso y les avisa automáticamente.
**Resultado:** Cero horas de administración al mes. El Churn se redujo un 15% gracias a los reintentos automáticos de tarjetas. El dueño ahora solo abre Stripe para mirar cuánto ha facturado mientras dormía.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
