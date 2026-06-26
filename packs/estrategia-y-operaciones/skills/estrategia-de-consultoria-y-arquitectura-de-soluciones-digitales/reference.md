# Referencia ampliada — Estrategia de Consultoría y Arquitectura de Soluciones Digitales (Principal Solution Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de diseño sistémico.*

1.  **Trigger:** Se inicia un nuevo proyecto o se solicita un cambio mayor de arquitectura en un sistema existente.
2.  **Nodo de Extracción de Requerimientos:** IA analiza la documentación de negocio y extrae las limitaciones técnicas (Presupuesto, Carga esperada, Time-to-market).
3.  **Nodo de Simulación de Soluciones:** El sistema genera 3 alternativas de arquitectura comparando costes, velocidad de desarrollo y escalabilidad.
4.  **Nodo de Validación Contra Estándares:** Se comprueba que la solución elegida cumple con los principios de Antigravity (Premium, Seguro, Eficiente).
5.  **Output:** Blueprint técnico completo enviado al equipo de desarrollo; creación automática de los registros de decisión de arquitectura iniciales.

---

## 7. Ejemplo Práctico: Marketplace Global de Logística
**Reto:** El sistema original colapsaba en el Black Friday y no permitía añadir nuevos proveedores sin reescribir media App.
**Acción v2.0:** Se rediseñó la solución hacia una arquitectura orientada a eventos (Event Driven) utilizando funciones serverless para los picos de carga.
**Resultado:** Cero caídas en el siguiente periodo de alta demanda. El tiempo de integración de un nuevo proveedor bajó de 4 semanas a 3 días, permitiendo a la empresa captar el 50% de la cuota de mercado en su nicho.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
