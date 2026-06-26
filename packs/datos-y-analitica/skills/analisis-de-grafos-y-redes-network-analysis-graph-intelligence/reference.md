# Referencia ampliada — Análisis de Grafos y Redes (Network Analysis & Graph Intelligence)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de monitorización relacional.*

1.  **Trigger:** Creación de una nueva conexión o registro en el sistema (Ej: Nueva transacción bancaria).
2.  **Nodo de Enriquecimiento de Grafo:** El sistema inserta el nuevo nodo y arista en la base de datos de grafos en tiempo real.
3.  **Nodo de Análisis de Patrones por IA:** El sistema ejecuta algoritmos de búsqueda de ciclos o patrones de fraude predefinidos.
4.  **Nodo de Alerta de Conexión Crítica:** Si se detecta que el nuevo nodo conecta dos comunidades previamente aisladas de alto riesgo, se dispara una alerta.
5.  **Output:** Grafo actualizado y visualizable; equipo de seguridad o estrategia informado sobre cambios críticos en la topología del sistema.

---

## 7. Ejemplo Práctico: Aseguradora 'SafeDrive'
**Reto:** Sufrieron un ataque de fraude coordinado. Individuos reclamaban accidentes falsos. En base de datos normal, todos los datos eran diferentes (nombres, matrículas).
**Acción v2.0:** Pasaron los datos a un grafo. La IA detectó que 12 personas "diferentes" habían usado el mismo número de móvil de contacto en los últimos 2 años, conectadas a través de 3 peritos comunes.
**Resultado:** Desarticularon una red de fraude de 500.000€. El análisis relacional detectó lo que la búsqueda por campos individuales nunca habría visto.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
