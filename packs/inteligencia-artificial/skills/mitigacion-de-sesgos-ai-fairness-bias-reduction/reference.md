# Referencia ampliada — Mitigación de Sesgos (AI Fairness & Bias Reduction)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de purificación algorítmica.*

1.  **Trigger:** Finalización del entrenamiento de un modelo o llegada de un nuevo lote de datos de producción.
2.  **Nodo de Auditoría Automática de Equidad:** El sistema ejecuta una batería de tests de impacto dispar comparando las predicciones del modelo entre diferentes subgrupos demográficos.
3.  **Nodo de Mitigación Activa:** Si se detecta un sesgo por encima del umbral permitido, el sistema activa automáticamente una capa de re-calibración de umbrales para ese grupo específico.
4.  **Nodo de Informe de Conformidad:** IA redacta un reporte técnico de "Certificado de Equidad" detallando las métricas alcanzadas y las acciones tomadas.
5.  **Output:** Modelo calibrado y listo para despliegue; alerta al administrador si el sesgo es tan profundo que requiere una re-arquitectura total de los datos de origen.

---

## 7. Ejemplo Práctico: App de Microcréditos 'FinEquity'
**Reto:** Su IA aprobaba préstamos con un interés mucho más alto a jóvenes menores de 25 años, asumiendo que eran "menos responsables", a pesar de tener ingresos estables.
**Acción v2.0:** Implementaron Mitigación de Sesgos (Skill 210). Realizaron un re-pesaje de los datos de entrenamiento para eliminar el prejuicio de edad y aplicaron una calibración de umbrales para asegurar igualdad de oportunidades.
**Resultado:** La tasa de aprobación de jóvenes solventes subió un 35% sin aumentar la morosidad del fondo. La empresa fue premiada por su enfoque de "Inclusión Financiera Guiada por IA".

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
