# Referencia ampliada — Estrategia de Product Analytics y Métricas de Negocio (Behavioral Data Strategy)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de inteligencia de datos.*

1.  **Trigger:** Ocurre un evento significativo de usuario o se llega al final de un periodo de reporte (Semanal/Mensual).
2.  **Nodo de Procesamiento y Atribución:** El sistema limpia los datos, asigna el usuario a su cohorte y calcula las métricas de conversión.
3.  **Nodo de Detección de Insights:** IA analiza los datos buscando correlaciones inusuales (Ej: "Los usuarios que usan la función X tienen una retención un 40% superior").
4.  **Nodo de Generación de Reporte Automatizado:** El sistema crea un resumen ejecutivo con las 3 recomendaciones de mejora de producto basadas en los datos detectados.
5.  **Output:** Información accionable entregada al equipo de producto; el ciclo de aprendizaje se cierra y el roadmap se ajusta dinámicamente.

---

## 7. Ejemplo Práctico: App de Gestión de Dietas
**Reto:** Tenían muchos registros pero solo el 10% de los usuarios ponía su primera comida del día.
**Acción v2.0:** El análisis de analytics detectó que el formulario de registros de comida tenía 12 campos. El experimento propuso reducirlo a 2 campos (Nombre y Foto).
**Resultado:** La activación (primera comida registrada) subió del 10% al 65%. La retención al mes siguiente se duplicó gracias a la reducción de la fricción inicial.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
