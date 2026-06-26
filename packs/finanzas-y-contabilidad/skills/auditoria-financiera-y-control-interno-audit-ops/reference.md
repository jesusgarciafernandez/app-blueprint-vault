# Referencia ampliada — Auditoría Financiera y Control Interno (Audit Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Ingeniería del Sistema de Control Preventivo
**Objetivo:** Crear el "sistema inmunológico" financiero de la empresa.
1.  **Mapeo de Riesgos por Centro de Coste (IA):** Identificación de dónde es más probable que ocurra un error o un fraude según el sector.
2.  **Configuración de Reglas de validación 'Hard' y 'Soft':** Bloqueos de sistema para transacciones críticas.

**Prompt Maestro de Fiscalización Financiera (Audit Architect):**
```text
Actúa como un Senior Auditor Forense y Experto en Control Interno. Vamos a auditar el ciclo de [COMPRAS/VENTAS] de [EMPRESA]. 
1. Diseño de Matriz de Riesgos IA: Basado en este historial de transacciones [DATOS], identifica los 3 patrones de comportamiento que se desvían de la norma y que podrían indicar fraude o error de registro. 
2. Guion de Prueba de Reconciliación: Diseña el flujo automático para comparar los cobros en Stripe con los pedidos en Shopify y los asientos en el Libro Diario. ¿Dónde están los descuadres? 
3. Auditoría de 'Gatos Fantasma': Busca proveedores cuyas facturas lleguen siempre cerca de los límites de aprobación manual o que tengan datos de contacto similares a los de nuestros empleados. 
4. Validación de Valoración de Existencias/Activos: Comprueba si la amortización aplicada este año cumple con la normativa [NORMATIVA] para estos activos específicos. 
5. Protocolo de 'Certificación de Cuentas': ¿Qué documentación y evidencias digitales debo generar hoy para que la auditoría externa obligatoria del próximo año sea un trámite de 1 hora?
```

### Fase 2: Ejecución, Inspección Profunda y Refactorización del Cumplimiento
... (Expansión técnica sobre el uso de la técnica de 'Minería de Procesos Financieros', la implementación de un proceso de 'Auditoría de Algoritmos Contables', y la monitorización de la 'Métrica de Tasa de Error en el Registro (Journal Entry Error Rate)' para asegurar que la organización es un templo de la integridad económica) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control operativa.*

1.  **Trigger:** Registro de asiento contable de alto importe, cambio en el maestro de proveedores, o cierre de periodo fiscal.
2.  **Nodo de Verificación de Reglas (Compliance Engine):** La IA comprueba que el asiento cuadra, tiene factura adjunta y el proveedor es de confianza.
3.  **Nodo de Detección de Anomalías (AI Forensics):** Comparativa estadística del gasto con el presupuesto y con meses anteriores para detectar picos injustificados.
4.  **Nodo de Reporte de Control y Escalamiento:** Si hay sospecha, se detiene el flujo de pago y se envía una alerta al responsable de cumplimiento (Compliance Officer).
5.  **Output:** Información financiera 100% fiable; eliminación del riesgo de fraude; cumplimiento normativo perfecto; tranquilidad absoluta para socios e inversores.

---

## 7. Ejemplo Práctico: La Empresa de Distribución 'Fast-Log'
**Reto:** 'Fast-Log' creció muy rápido. Tenían 500 empleados con tarjetas de empresa. La revisión de los gastos se hacía un mes después por un equipo pequeño. Un gestor de almacén estuvo pasando facturas personales de "material de mantenimiento" durante un año por valor de 50.000€ que nadie detectó porque eran importes pequeños repartidos en muchos días.
**Acción v2.0:** Implementaron Skill 342. La IA empezó a analizar cada ticket de mantenimiento. El sistema detectó que un proveedor nuevo de ferretería tenía la misma dirección fiscal que la casa del gestor de almacén. La alerta saltó en la tercera factura.
**Resultado:** Se detuvo el fraude en seco. Además, descubrieron que el 10% de los tickets de gasolina de los repartidores tenían errores de IVA, lo que les permitía recuperar 5.000€ extra al año que antes se perdían por mala contabilidad. 'Fast-Log' ahora es una empresa "a prueba de balas" financiera.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
