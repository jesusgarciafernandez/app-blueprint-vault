# Referencia ampliada — Gestión del Presupuesto y Control de Costes (Budget Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Diagnóstico del Burn Rate y Configuración del Plan Maestro
**Objetivo:** Saber cuánto oxígeno (dinero) queda y cómo vamos a usarlo.
1.  **Auditoría de Suscripciones e Ineficiencias (IA):** El agente escanea los extractos bancarios buscando duplicados, herramientas SaaS no usadas y fugas de capital menores.
2.  **Mapeo de Centros de Gasto Estratégicos:** Clasificación de cada gasto según si es 'Inversión Crecimiento', 'Coste Mantenimiento' o 'Desperdicio'.

**Prompt Maestro de Arquitectura Presupuestaria (Budget Architect):**
```text
Actúa como un Senior CFO y Experto en Lean Finance. Ayúdame a optimizar el presupuesto para [EMPRESA/PROYECTO]. 
1. Auditoría de 'Inercias' Financieras: Basado en este historial de gastos [DATOS], identifica 5 gastos que se han vuelto 'invisibles' y que podríamos eliminar sin afectar la operativa. 
2. Diseño de Presupuesto Base Cero: Guíame para reconstruir el presupuesto de [DEPARTAMENTO] desde cero. ¿Qué preguntas debo hacer por cada línea de gasto para validar su necesidad estratégica? 
3. Simulación de Estrés Financiero: Crea 3 escenarios de caja: A) Escenario Optimista (crecimiento 20%), B) Escenario Estable, C) Escenario de Crisis (caída de ingresos del 40%). ¿Qué recortes de emergencia activaríamos en C? 
4. Regla de Alerta de Desviación: Define los umbrales (ej: 5% de desviación) y el mensaje de alerta que la IA me enviará al móvil cada vez que un centro de coste se pase de la raya. 
5. Protocolo de 'Inversión por Rendimiento': ¿Cómo configuro un sistema que asigne más presupuesto automáticamente al canal de marketing que mejor ROI esté dando hoy?
```

### Fase 2: Ejecución, Monitorización de Flujo y Refactorización del Rendimiento
... (Expansión técnica sobre el uso de la técnica de 'Allocation Dinámica de Recursos', la implementación de un proceso de 'Auditoría de Gastos en la Sombra', y la monitorización de la 'Métrica de Eficiencia del Capital (Burn Multiple)' para asegurar que la organización es una máquina financieramente robusta y enfocada) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control operativa.*

1.  **Trigger:** Registro de un nuevo gasto en el sistema contable, finalización del mes fiscal, o detección de un saldo bancario por debajo del umbral de seguridad.
2.  **Nodo de Clasificación y Comparativa:** La IA compara el gasto real con la partida presupuestaria asignada para ese mes/categoría.
3.  **Nodo de Re-Forecasting Automático:** Si un proyecto gasta menos de lo previsto, el sistema propone redistribuir ese sobrante a otro proyecto bloqueado por falta de fondos.
4.  **Nodo de Reporte de 'Salud Presupuestaria':** Generación de un PDF ejecutivo semanal con el semáforo de gastos (Verde: OK, Amarillo: Alerta, Rojo: Desviación crítica).
5.  **Output:** Control total sobre el Burn Rate; eliminación del desperdicio financiero; aumento del retorno de la inversión; tranquilidad y solvencia estratégica.

---

## 7. Ejemplo Práctico: El caso de la Agencia 'Creativa X'
**Reto:** 'Creativa X' facturaba mucho, pero el dueño siempre sentía que no tenía dinero en el banco. Tenían decenas de suscripciones a software de diseño, stocks innecesarios y gastaban mucho en "comidas de empresa" sin control. El presupuesto se hacía una vez al año y nadie lo miraba hasta diciembre.
**Acción v2.0:** Implementaron Skill 336. Instalaron un Agente que clasificaba los gastos en tiempo real desde la tarjeta corporativa. La IA detectó que pagaban por 5 herramientas similares y que las comidas sumaban el sueldo de un diseñador junior al mes. Pasaron a un Presupuesto Base Cero.
**Resultado:** En solo 2 meses, el Burn Rate bajó un 15% sin despedir a nadie ni afectar la calidad del trabajo. El dinero ahorrado se invirtió en una formación avanzada para el equipo, lo que permitió subir los precios de sus servicios. Ahora, el dueño tiene un semáforo en su pantalla: mientras esté en verde, sabe que la empresa es rentable y segura.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
