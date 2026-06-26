# Referencia ampliada — Data Mining & Knowledge Discovery (Extracción de Inteligencia de Datos)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de descubrimiento continuo.*

1.  **Trigger:** Carga semanal de grandes datasets históricos de transacciones o interacciones.
2.  **Nodo de Reducción y Limpieza:** El sistema filtra datos irrelevantes y prepara el formato "transaccional" para la minería.
3.  **Nodo de Ejecución Alogritmo de Minería:** IA busca automáticamente patrones de asociación y secuencias con alta confianza.
4.  **Nodo de Filtrado de Novedad:** El sistema compara los patrones encontrados con los conocidos, resaltando solo los "nuevos" descubrimientos.
5.  **Output:** Informe de "Nuevos Insights de Negocio"; alerta automática al equipo de estrategia si se detecta un cambio brusco en los patrones habituales de los clientes.

---

## 7. Ejemplo Práctico: Supermercado Online 'FreshClick'
**Reto:** Sus promociones de "2x1" no funcionaban. Enviaban cupones de pañales a gente que no los compraba habitualmente.
**Acción v2.0:** Hicieron Data Mining de 2 años de tickets. La IA descubrió que los clientes de "comida orgánica" tenían una alta asociación (Lift) con la compra de "detergentes ecológicos", aunque fueran categorías separadas.
**Resultado:** Hicieron campañas cruzadas. La facturación de detergentes subió un 40% al impactar al nicho de "estilo de vida consciente" identificado por la minería.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
