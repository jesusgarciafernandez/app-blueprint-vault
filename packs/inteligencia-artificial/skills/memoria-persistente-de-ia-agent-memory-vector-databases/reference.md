# Referencia ampliada — Memoria Persistente de IA (Agent Memory & Vector Databases)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de cognición persistente.*

1.  **Trigger:** Entrada del usuario o evento del sistema que requiere recuperar información histórica.
2.  **Nodo de 'Query Expansion' por IA:** El sistema analiza la entrada y genera varias consultas semánticas para cubrir diferentes ángulos de la memoria.
3.  **Nodo de Búsqueda Vectorial:** Se realiza la búsqueda en la DB de largo plazo y se obtienen los fragmentos de memoria más cercanos.
4.  **Nodo de Síntesis y Re-contextualización:** IA integra los recuerdos recuperados en el pensamiento actual del agente para generar una respuesta coherente.
5.  **Output:** Respuesta personalizada que demuestra memoria; el sistema registra el nuevo intercambio para convertirlo en memoria futura tras el proceso de resumen.

---

## 7. Ejemplo Práctico: Agencia de Diseño 'StudioMemory'
**Reto:** Sus agentes creativos de IA olvidaban el estilo visual de los clientes entre una reunión y otra, lo que obligaba a los humanos a re-explicar las guías de marca constantemente.
**Acción v2.0:** Implementaron Memoria Persistente (Skill 198). Cada vez que un cliente daba feedback sobre un color o tipografía, el agente guardaba el "Voto Preferencial" en su memoria de largo plazo.
**Resultado:** En la siguiente sesión, el agente ya sabía que al cliente no le gustaba el rojo pastel, ahorrando horas de retrabajo. El sistema se volvió cada vez más eficiente a medida que "conocía" más a cada director de arte.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
