# Referencia ampliada — Operaciones de Ventas (SalesOps Performance Mastery)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de soporte operativo.*

1.  **Trigger:** Un lead entra en el sistema o un deal cambia de etapa en el CRM de forma manual.
2.  **Nodo de Clasificación y Routing:** El sistema asigna automáticamente el lead al vendedor disponible con mejor historial para esa categoría de cliente.
3.  **Nodo de Enriquecimiento de Datos:** IA busca el perfil de LinkedIn y noticias recientes de la empresa del prospecto para dar contexto al vendedor.
4.  **Nodo de Seguimiento de Actividad:** Registro automático de correos y llamadas; si no hay actividad en 48h, se dispara un aviso al Sales Manager.
5.  **Output:** Pipeline actualizado y limpio; el equipo comercial recibe leads pre-calificados y listos para la llamada.

---

## 7. Ejemplo Práctico: Startup Ganadera con Ventas B2B
**Reto:** Los vendedores olvidaban hacer seguimiento a los leads de ferias agrícolas porque tenían que meter los datos a mano en un Excel. Perdían el 70% de las oportunidades por tardar 1 semana en llamar.
**Acción v2.0:** Se implementó una App de escaneo de tarjetas vinculada al CRM. El lead recibía un email de bienvenida automático a los 10 minutos de la feria. El vendedor recibía una tarea de "Llamada Prioritaria" al llegar a la oficina.
**Resultado:** El tiempo de primer contacto bajó de 7 días a 1 hora. Las ventas en el siguiente trimestre subieron un 50% solo por "estar ahí primero".

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
