# Referencia ampliada — Onboarding Autoservicio SaaS (Zero-Touch Provisioning)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de despliegue de cliente.*

1.  **Trigger:** Éxito en la suscripción (Evento de pago confirmado en Stripe/PayPal).
2.  **Nodo de Orquestador de Infraestructura:** Disparo de lambdas o scripts que crean los recursos técnicos aislados para el nuevo cliente.
3.  **Nodo de Inyección de Semántica Inicial:** IA genera los primeros datos, proyectos o tareas según la industria que seleccionó el usuario al registrarse.
4.  **Nodo de Comunicación de Bienvenida:** Envío de credenciales seguras y acceso al enlace del tour inicial.
5.  **Output:** Entorno listo para usar; el contador de 'Tiempo para el Valor' (TTV) empieza a correr.

---

## 7. Ejemplo Práctico: SaaS de Facturación para Pequeñas Empresas
**Reto:** El 60% de los usuarios se registraba pero no configuraba su primer cliente ni su logo, por lo que nunca llegaban a facturar y cancelaban.
**Acción v2.0:** Se implementó un asistente de "Configuración en 3 pasos". En el paso #1, la IA extraía el logo y datos fiscales de la web del usuario solo con su URL. El entorno aparecía ya "personalizado" en el primer login.
**Resultado:** La tasa de activación subió un 45%. El usuario se sentía "dentro de su propia herramienta" desde el primer segundo.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
