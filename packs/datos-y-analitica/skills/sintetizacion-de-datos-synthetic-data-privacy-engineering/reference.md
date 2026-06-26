# Referencia ampliada — Sintetización de Datos (Synthetic Data & Privacy Engineering)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Entrenamiento del Modelo Generador
**Objetivo:** Capturar la esencia estadística de los datos reales.
1.  **Perfilado de Metadatos y Restricciones:** IA ayuda a mapear las reglas lógicas (Ej: "La fecha de muerte debe ser posterior a la de nacimiento") que el modelo sintético debe heredar.
2.  **Entrenamiento del Optimizador:** Proceso de ajuste de redes neuronales (GANs) para minimizar la distancia entre la distribución real y la generada.

**Prompt Maestro de Sintetización de Datos:**
```text
Actúa como un Senior Synthetic Data Engineer y Experto en Privacy Engineering. Facilita la creación del dataset sintético para [TIPO_DE_DATO]. 
1. Analiza el Dataset Real: Identifica las correlaciones críticas que el modelo DEBE mantener (Ej: Relación entre [VAR_A] y [VAR_B]). 
2. Configura el Generador (SDV): Genera el script en Python para entrenar un modelo 'GaussianCopula' o 'TVAE' basándose en los metadatos reales. 
3. Informe de Fidelidad (Fidelity Report): ¿Qué métricas de similitud estadística (CS Test, Likelihood) sugieres para validar que el dato sintético es útil para el análisis? 
4. Evaluación de Privacidad (Privacy Score): Realiza un test de riesgo de re-identificación buscando 'registros gemelos' entre el original y el sintético. 
5. Dataset de Salida: Genera [Nº_REGISTROS] y exporta a [FORMATO] asegurando que no queden restos de información personal en los metadatos.
```

### Fase 2: Validación, Despliegue y Auditoría
... (Expansión técnica sobre el uso de la 'Distancia de Jensen-Shannon' para comparar distribuciones, la implementación de pipelines de sintetización en tiempo real para flujos de datos dinámicos y la creación de certificados de privacidad que garanticen que el dataset resultante cumple con las normativas de 'Anonimización Irreversible') ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de creación de gemelos digitales.*

1.  **Trigger:** Solicitud de acceso a datos protegidos por parte de un equipo de desarrollo o investigador.
2.  **Nodo de Entrenamiento 'Secure-Buffer':** En un entorno aislado, la IA entrena el modelo generativo sobre el dataset real crudo.
3.  **Nodo de Generación Sintética:** El sistema produce una versión artificial del dataset que respeta todas las restricciones lógicas y estadísticas.
4.  **Nodo de Auditoría de Privacidad por IA:** Un tercer proceso verifica que no hay registros idénticos al original y que el riesgo de fuga es despreciable.
5.  **Output:** Dataset sintético entregado al solicitante; el original permanece inaccesible y seguro en el vault corporativo.

---

## 7. Ejemplo Práctico: Banco 'SecureFinance'
**Reto:** Necesitaban que una consultora externa probara un modelo de detección de blanqueo de capitales, pero por ley no podían enviarles los movimientos bancarios de sus clientes reales.
**Acción v2.0:** Aplicaron Sintetización de Datos (Skill 191). Generaron 1 millón de transacciones sintéticas que imitaban perfectamente los patrones de gasto y fraude del banco.
**Resultado:** La consultora desarrolló el modelo sobre el dato sintético. Cuando el banco lo aplicó a los datos reales, funcionó con un 98% de la precisión esperada, todo ello sin que un solo dato de cliente real saliera jamás del firewall del banco.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
