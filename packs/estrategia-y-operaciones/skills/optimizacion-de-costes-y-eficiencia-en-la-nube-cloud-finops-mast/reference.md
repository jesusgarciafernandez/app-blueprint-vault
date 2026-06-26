# Referencia ampliada — Optimización de Costes y Eficiencia en la Nube (Cloud FinOps Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control financiero.*

1.  **Trigger:** El cierre diario de facturación detecta un recurso con un coste >X€ que no cumple con las políticas de etiquetado o está infrautilizado (<10% CPU).
2.  **Nodo de Evaluación de Impacto:** El sistema comprueba si el recurso es crítico para producción o es de un entorno de pruebas.
3.  **Nodo de Acción Sugerida / Ejecutada:** El sistema envía un aviso al dueño del recurso con un botón de "Optimizar ahora" o lo apaga automáticamente si es fuera de horario laboral en desarrollo.
4.  **Nodo de Reporte de Ahorro:** Se calcula el dinero ahorrado por la acción y se suma al contador mensual de eficiencia.
5.  **Output:** Factura controlada y optimizada; el equipo de ingeniería recibe medallas de eficiencia basadas en sus ahorros conseguidos.

---

## 7. Ejemplo Práctico: Fintech con Microservicios en Kubernetes
**Reto:** Su factura de AWS crecía un 20% al mes mientras su número de clientes solo crecía un 5%. Estaban perdiendo el margen de beneficio por mala gestión de Kubernetes.
**Acción v2.0:** Se implementó Kubecost para asignar costes por microservicio y se detectó que el servicio de "Generación de Documentos" consumía el 40% del gasto por estar mal programado y no escalar hacia abajo. Se refactorizó ese servicio y se movió a instancias Spot.
**Resultado:** La factura cloud bajó un 35% en el primer mes y el margen de beneficio por cada cliente nuevo subió un 25%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
