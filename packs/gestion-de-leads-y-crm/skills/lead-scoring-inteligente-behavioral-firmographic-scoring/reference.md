# Referencia ampliada — Lead Scoring Inteligente (Behavioral & Firmographic Scoring)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de clasificación y alerta.*

1.  **Trigger:** El usuario realiza una acción digital (Web, Email, Evento) o actualiza un dato en su ficha.
2.  **Nodo de Cálculo de Puntuación:** El sistema evalúa instantáneamente la nueva acción y la suma a la puntuación acumulada, aplicando reglas de 'Time Decay' si corresponde.
3.  **Nodo de Evaluación de Umbral:** ¿Ha superado el lead la puntuación de 100 puntos (Sales Ready)?
4.  **Nodo de Acción de Prioridad:** Si se supera el umbral, se cambia el estado a "MQL" y se envía una notificación push al móvil del comercial asignado.
5.  **Output:** Pipeline priorizado; el comercial se enfoca en el lead calificado mientras el sistema sigue nutriendo al resto.

---

## 7. Ejemplo Práctico: Empresa de Software ERP
**Reto:** Recibían 2000 leads al mes, pero el equipo de ventas solo podía llamar a 10 personas al día. Llamaban por orden de llegada y perdían las oportunidades realmente buenas.
**Acción v2.0:** Se implementó scoring. Se dio prioridad máxima (+50 pts) a quienes visitaran la página de "Comparativa con Competencia" y "Precios". Se restaron 100 puntos a dominios @gmail.com o @yahoo.com.
**Resultado:** Los comerciales empezaron a llamar a leads con una tasa de cierre del 10% (antes era del 1%). Las ventas subieron un 300% con el mismo equipo humano.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
