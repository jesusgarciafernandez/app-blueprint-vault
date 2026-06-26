# Referencia ampliada — Diseño de Servicios (Service Design), Service Blueprint y Orquestación de Ecosistemas

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de orquestación de servicios automatizada.*

1.  **Trigger:** Un sensor IoT en una máquina de vending detecta que el stock de café se está agotando.
2.  **Nodo de Backstage Automático:** El sistema genera una orden de reposición, optimiza la ruta del técnico más cercano y actualiza la App de usuarios avisando de: "Reponiendo granos frescos en 15 min".
3.  **Nodo de Verificación de Compromiso (SLA):** IA monitoriza si el técnico llega a tiempo. Si no, activa una compensación automática por fidelidad al siguiente usuario que compre.
4.  **Nodo de Análisis de Feedback:** El sistema recoge el sentimiento post-compra y lo asocia a la eficiencia de esa ruta logística específica.
5.  **Output:** Dashboard de "Salud del Servicio" que avisa de problemas operativos antes de que el cliente final llegue a percibirlos como una mala experiencia.

---

## 7. Ejemplo Práctico: Rediseño de Clínica Dental Premium
**Reto:** Los pacientes estaban contentos con el dentista, pero odiaban la espera en recepción y la confusión con los presupuestos, lo que bajaba la aceptación de tratamientos.
**Acción v2.0:** Se rediseñó el servicio completo. La App permite hacer el registro previo. Al llegar, recepción ya tiene todo listo. El presupuesto se explica con un video 3D personalizado generado por IA.
**Resultado:** Los tiempos de espera bajaron un 50% y la tasa de aceptación de presupuestos subió un 35%, no por mejorar el trabajo dental, sino por mejorar la orquestación del servicio previo y posterior.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
