# Referencia ampliada — Estrategias de Retención y Prevención de Churn (Retention Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de salvaguarda de clientes.*

1.  **Trigger:** El Health Score de un cliente cae por debajo de un umbral crítico o se detecta un patrón de abandono (Ej: Desinstalación de plugin).
2.  **Nodo de Clasificación de Causa:** IA analiza el contexto (Ej: ¿Ha tenido muchos tickets de error? ¿Ha bajado su uso drásticamente?).
3.  **Nodo de Acción Sugerida:** El sistema decide entre disparar un flujo de re-onboarding automático o asignar una llamada de urgencia al Customer Success Manager.
4.  **Nodo de Monitorización de Respuesta:** Se rastrea si la intervención surte efecto y el Score vuelve a subir en los siguientes 7 días.
5.  **Output:** Reporte de 'Vidas Salvadas' y aprendizaje sobre las causas de riesgo para optimizar el producto y evitar futuros casos similares.

---

## 7. Ejemplo Práctico: SaaS de CRM para Inmobiliarias
**Reto:** Los agentes dejaban de usar la App después de la primera semana porque les parecía difícil subir las fotos de los pisos. El Churn era del 15% mensual.
**Acción v2.0:** Se detectó que quien usaba la App móvil para las fotos en las primeras 48h tenía una retención de 1 año. Se automatizó un aviso al móvil: "¡Hola! He visto que has captado un piso, ¿quieres que te ayude a subir las fotos ahora desde aquí?".
**Resultado:** El uso de la App móvil subió un 300% y el Churn cayó al 4% en solo dos meses.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
