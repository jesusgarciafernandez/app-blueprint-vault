# Referencia ampliada — Agentes de Computer Use (UI-Driven Agents & OS Control)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de operación visual continua.*

1.  **Trigger:** Solicitud de tarea administrativa o detección de un cambio de estado en un sistema monitorizado.
2.  **Nodo de Percepción Visual:** El sistema captura el estado actual de la pantalla del entorno sandbox.
3.  **Nodo de Razonamiento Táctico IA:** El modelo procesa la imagen, decide la siguiente acción (mover mouse, click, escribir) y envía la instrucción.
4.  **Nodo de Ejecución de Periféricos:** Un driver del sistema operativo ejecuta la acción física sobre la interfaz.
5.  **Output:** Tarea completada en la interfaz real; el sistema guarda el vídeo del proceso para validación del humano y confirmación de éxito.

---

## 7. Ejemplo Práctico: Agencia 'TotalAdmin'
**Reto:** Al día recibían 100 facturas en formatos PDF distintos que debían subir manualmente a un software de contabilidad de 1995 que no tiene API ni base de datos accesible.
**Acción v2.0:** Implementaron un Agente de Computer Use (Skill 197). La IA abría la factura, "veía" el importe, abría el programa antiguo, navegaba por los menús grises y tecleaba los datos uno a uno.
**Resultado:** El proceso pasó de tardar 8 horas diarias de un humano a 20 minutos de ejecución autónoma. El humano ahora solo revisa el log visual de la IA para asegurar que todo cuadra.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
