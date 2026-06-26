# Referencia ampliada — Desarrollo de Superagente Comercial B2B (Autonomous SDR Agent)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de prospección inteligente.*

1.  **Trigger:** El CRM detecta un nuevo prospecto en una cuenta objetivo o se lanza una nueva lista de enriquecimiento.
2.  **Nodo de Investigación Autónoma:** El Agente "Scout" rastrea la web buscando evidencias de necesidad (Ej: Ofertas de empleo activas, nuevas rondas de inversión).
3.  **Nodo de Composición de Mensaje:** El Agente "Writer" crea una propuesta de valor única vinculando la necesidad detectada con la solución del SaaS.
4.  **Nodo de Envío y Monitorización:** El sistema envía el mensaje y monitoriza la respuesta; si es positiva, agenda la reunión; si es negativa, aprende y actualiza el perfil del lead.
5.  **Output:** Agenda comercial llena de reuniones de alta calidad; reporte de 'Inteligencia de Mercado' generado a partir de las investigaciones del agente.

---

## 7. Ejemplo Práctico: SaaS de Ciberseguridad para Fintech
**Reto:** Prospección a CTOs de bancos, un perfil muy saturado que ignora correos genéricos.
**Action v2.0:** Se desarrolló un superagente que leía las últimas noticias sobre brechas de seguridad en el sector del banco objetivo y personalizaba el correo mencionando cómo su software habría evitado ese caso específico.
**Resultado:** La tasa de respuesta positiva subió del 0.5% al 12%. El equipo de ventas pasó de hacer 100 llamadas frías a tener 5 reuniones de alta importancia a la semana generadas por el agente.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
