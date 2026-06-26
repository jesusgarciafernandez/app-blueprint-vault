# Referencia ampliada — Diseño Estratégico Orientado al Dominio (Domain-Driven Design / DDD)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Descubrimiento del Dominio y Bounded Contexts
**Objetivo:** Entender el negocio antes de tocar una sola línea de código.
1.  **Auditoría de Lenguaje:** IA ayuda a extraer los términos clave de los documentos de negocio y proponer un glosario de 'Lenguaje Ubicuo'.
2.  **Mapeo de Contextos (Strategic Design):** Identificación de las áreas con responsabilidades independientes dentro de la organización.

**Prompt Maestro de Modelado DDD (Domain Architect):**
```text
Actúa como un Senior Software Architect y Experto en Domain-Driven Design. Diseña el modelo estratégico para el dominio: [DESCRIPCIÓN_NEGOCIO]. 
1. Identificación de Bounded Contexts: Define al menos 3 contextos independientes (Ej: Catálogo, Pedidos, Envios) y justifica sus fronteras. 
2. Glosario de Lenguaje Ubicuo: Lista los 5 términos más importantes para este negocio y define qué significan exactamente en el contexto del software. 
3. Diseño de Agregados Tácticos: Para el contexto [CONTEXTO_X], identifica el 'Aggregate Root' y los 'Value Objects' que garantizan la integridad de la regla de negocio. 
4. Mapa de Contextos (Context Map): Describe cómo se comunicarán los contextos entre sí (Ej: Notificaciones vía Eventos, Llamadas síncronas con ACL - Anti-Corruption Layer). 
5. Taller de Event Storming: Diseña la agenda de una sesión para descubrir los eventos de dominio clave que disparan cambios en el sistema.
```

### Fase 2: Implementación Táctica y Refinamiento
... (Expansión técnica sobre el uso de la técnica de 'Dependency Inversion' para proteger el dominio de la base de datos, la implementación de un proceso de 'Domain Validation' donde los objetos no pueden crearse en un estado inválido, y la monitorización de la 'Fidelidad del Modelo' para asegurar que el código sigue siendo un reflejo exacto de los cambios en los procesos de negocio reales) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de alineamiento organizacional.*

1.  **Trigger:** Necesidad de implementar una nueva funcionalidad de negocio compleja o modificar un proceso existente.
2.  **Nodo de Traducción de Conceptos:** IA ayuda a traducir los requerimientos del experto en cambios específicos sobre el modelo de dominio y el lenguaje ubicuo.
3.  **Nodo de Validación de Fronteras:** El sistema verifica que la nueva funcionalidad pertenezca al 'Bounded Context' correcto y no ensucie otros módulos.
4.  **Nodo de Implementación Táctica:** Se codifican los cambios en las Entidades y Agregados, protegiendo las reglas de negocio mediante tests de dominio puros.
5.  **Output:** Software funcional que habla el idioma del negocio; documentación arquitectónica actualizada según la evolución del modelo de dominio.

---

## 7. Ejemplo Práctico: Operador Logístico 'GlobalShip'
**Reto:** En 'GlobalShip', la palabra "Envío" significaba cosas distintas para el camionero, el contable y el cliente. El código era una maraña de ifs para intentar contentar a todos, lo que hacía que cualquier cambio tardara meses.
**Acción v2.0:** Implementaron DDD (Skill 237). Crearon tres contextos claros: *Operaciones* (enfocado en rutas), *Facturación* (enfocado en costes) y *Customer Experience* (enfocado en tracking). Usaron una capa de traducción (ACL) para que se comunicaran.
**Resultado:** La velocidad de desarrollo aumentó un 300%. Los errores de facturación desaparecieron porque el código de facturación ya no dependía de los cambios en las rutas de los camiones. El negocio y el software finalmente hablaban el mismo idioma.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
