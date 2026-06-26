# Referencia ampliada — Análisis de Negocio y Optimización de Procesos (Business Process Excellence)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de optimización continua.*

1.  **Trigger:** Se detecta un incremento en el tiempo de ciclo (Cycle Time) de un proceso crítico o una queja de cliente recurrente.
2.  **Nodo de Auditoría de Datos:** El sistema extrae automáticamente los tiempos de ejecución de cada etapa desde las herramientas de gestión (Jira/Trello/ERP).
3.  **Nodo de Diagnóstico de IA:** IA compara el rendimiento actual con el benchmark óptimo y señala exactamente dónde está el bloqueo (Ej: "Aprobación manual pendiente de media 48h").
4.  **Nodo de Propuesta de Mejora:** El sistema propone una automatización parcial (Ej: Autorización automática bajo ciertos criterios) y envía un informe de impacto al responsable.
5.  **Output:** Proceso recalibrado; el sistema monitoriza los 30 días siguientes para confirmar que la mejora se consolida y libera tiempo humano.

---

## 7. Ejemplo Práctico: Departamento de Compras B2B
**Reto:** Tardaban 15 días en dar el alta a un nuevo proveedor por el intercambio masivo de PDFs y validaciones manuales lentas.
**Acción v2.0:** Se mapeó el proceso y se descubrió que el 70% del tiempo era espera de respuesta. Se implementó un portal de autoservicio para proveedores con validación automática de documentos vía IA.
**Resultado:** El tiempo de alta bajó de 15 días a 48 horas. Se eliminó el 90% de la carga administrativa del departamento de compras, permitiéndoles negociar mejores precios en lugar de perseguir papeles.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
