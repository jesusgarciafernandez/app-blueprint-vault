# Referencia ampliada — Análisis de Atribución (Marketing ROI & Path-to-Purchase Engineering)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de orquestación de mérito.*

1.  **Trigger:** Ocurre una conversión de éxito (Venta confirmada) en el backend.
2.  **Nodo de Reconstrucción de Journey:** El sistema busca en el histórico de cookies y User-ID todos los touchpoints previos de ese usuario.
3.  **Nodo de Asignación por Algoritmo:** IA aplica el modelo elegido y reparte el valor económico de la venta entre los canales participantes.
4.  **Nodo de Actualización de Dashboards:** Los datos agregados se envían al informe de ROI consolidado.
5.  **Output:** Visión real de la rentabilidad por canal; el sistema avisa si un canal está infravalorado por reportes estándar de "último clic".

---

## 7. Ejemplo Práctico: E-commerce de Muebles de Lujo 'HomeDesign'
**Reto:** Invertían 10.000€/mes en Pinterest para captar atención, pero Google Ads se llevaba todas las medallas por "último clic". Querían cerrar Pinterest porque "no vendía".
**Acción v2.0:** Aplicaron atribución lineal y luego Data-Driven. Descubrieron que el 70% de las compras de alto valor empezaban con una imagen en Pinterest 20 días antes.
**Resultado:** Mantuvieron y optimizaron Pinterest. El volumen de ventas total subió un 25% al alimentar correctamente la parte superior del funnel. Sin este análisis, habrían matado su mejor fuente de nuevos clientes.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
