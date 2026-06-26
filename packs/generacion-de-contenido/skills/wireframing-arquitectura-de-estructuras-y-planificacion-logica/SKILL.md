---
name: wireframing-arquitectura-de-estructuras-y-planificacion-logica
description: "El Wireframing es la creación de los planos arquitectónicos de una interfaz digital. No es un \"dibujito\"; es Ingeniería de la Columna Vertebral Digital. Úsala para tareas de Generación de Contenido: wireframing, low-fidelity, information-architecture, ux-design, interface-structure, skeletal-design."
title: Wireframing, Arquitectura de Estructuras y Planificación Lógica
version: 2.0
author: Jesús García Fernández
website: jesusgarciafernandez.com
created: 2026-04-01
updated: 2026-04-17
category: 02. Generación de Contenido
subcategory: Diseño UI
tags: [wireframing, low-fidelity, information-architecture, ux-design, interface-structure, skeletal-design, flow-mapping, blueprinting, ia-wireframe-gen]

license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
notice: >
  Esta skill es de autoría original de Jesús García Fernández.
  Permitido su uso personal y educativo citando la fuente.
  Prohibida su venta, redistribución comercial o modificación
  sin autorización expresa del autor.
id: 080
---

## 0. Filosofía Human-Centric AI
*Esta habilidad construye los cimientos de la claridad, utilizando la tecnología para desnudar la interacción de adornos y centrarse en la eficacia del propósito humano.*

**El Rol del Humano:** El Arquitecto de Wireframes debe ser un "Estratega de la Estructura Pura". La IA puede generar esquemas de cajas y líneas basados en sitemaps, sugerir disposiciones de rejilla (grids) estándar y automatizar el espaciado, pero solo el humano puede imbuir al esquema de la "prioridad" real necesaria, decidir qué información debe sacrificarse para salvar la usabilidad y asegurar que el "esqueleto" digital soporte el peso de la estrategia de negocio y la facilidad de uso humana, evitando distracciones estéticas prematuras.
**Empoderamiento:** Usamos la tecnología para automatizar el ensamblado de componentes de baja fidelidad (Lo-Fi) y la creación de flujos conectados, permitiendo que el experto se centre en la jerarquía de la información y en la validación de la lógica operativa.

---

## 1. Descripción Detallada
El Wireframing es la creación de los planos arquitectónicos de una interfaz digital. No es un "dibujito"; es **Ingeniería de la Columna Vertebral Digital**. El enfoque v2.0 incorpora la **Estructuración Sistémica y la Planificación de la Carga Cognitiva**, donde se utilizan esquemas en blanco y negro para validar la navegación, la distribución de contenidos y la jerarquía focal antes de invertir un solo segundo en diseño visual (UI) o código, garantizando que el producto sea funcionalmente impecable por diseño.

## 2. Escenarios de Aplicación
- **Ideación y Conceptualización Inicial:** Exploración de 10 soluciones diferentes en una hora mediante bocetos rápidos (Crazy 8's).
- **Alineamiento de Lógica de Negocio:** Presentación de flujos a stakeholders para validar que el proceso (ej: un seguro médico) tiene todos los pasos necesarios.
- **Definición de Arquitectura de Información:** Organización de menús, submenús y buscadores en una estructura jerárquica clara.
- **Documentación para Ingeniería:** Entrega de "mapas de cajas" que explican qué hace cada botón y a dónde lleva, sin ambigüedades.
- **Testeo de Concepto Temprano:** Validación con usuarios si entienden "para qué sirve cada pantalla" sin distraerse con colores o fotos.

## 3. Requisitos de Implementación
- **Maestría en Jerarquía Visual y Grids:** Conocimiento de cómo guiar el ojo mediante el tamaño y la posición de las cajas (Layout).
- **Dominio de Herramientas Lo-Fi:** Figma (con librerías de wireframing), Whimsical, Miro, Balsamiq o el clásico "Lápiz y Papel".
- **Habilidad de Abstracción:** Capacidad de representar ideas complejas mediante geometrías simples que comunican función, no forma.

---

## 4. Diferencial: Boceto Rápido vs. Wireframe Estratégico v2.0

| Dimensión | Enfoque "Dibujo a mano" | Wireframing Estratégico (v2.0) |
| :--- | :--- | :--- |
| **Meta** | Visualizar la idea. | Validar la lógica y la jerarquía. |
| **Contenido** | "Lorem Ipsum" y fotos aleatorias. | Copy real (Draft) y placeholders de datos. |
| **Enlace** | Pantallas sueltas. | Flujos de usuario completos (User Flows). |
| **Precisión** | Despreocupada. | Píxel-perfect en espaciado (Estructural). |

---

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Definición de la Rejilla Estructural y Jerarquía Focal
**Objetivo:** Crear el contenedor lógico donde vivirá la información.
1.  **Establecimiento del Grid:** Define si usarás 12 columnas (Web) o 4 columnas (Mobile). Asegura los márgenes de seguridad.
2.  **Mapeo de Bloques de Contenido:** Coloca cajas para los elementos críticos: [Logo, Menú, Título, Texto de apoyo, Acción principal (CTA)].

**Prompt Maestro de Dirección de Wireframing:**
```text
Actúa como Especialista en Arquitectura de Información y Master de Wireframing. Para el flujo de [FLUJO], solicita el siguiente diseño estructural: 
1. Diseña el 'Esqueleto' de la Home: [Ej: Cabecera pegajosa, Sección Hero con caja de búsqueda central y Grid de 3 tarjetas de beneficios]. 
2. Establece la 'Jerarquía de Pesos': Usa grosores de línea y sombras en escala de grises para indicar qué elemento tiene prioridad 1, 2 y 3. 
3. Define los 'Placeholders' de Datos Reales: No uses Lorem Ipsum; pon textos cortos que expliquen qué información irá en cada caja. 
4. Documenta el 'Comportamiento de los Slots': Qué ocurre cuando esta caja no tiene datos o da un error. 
5. Protocolo de 'Fricción Mínima': Evalúa si se puede eliminar algún bloque o paso del flujo para simplificar la estructura.
```

### Fase 2: Conexión de Flujos, Revisión Estructural y Transición a Hi-Fi
... (Expansión técnica sobre el uso de 'Annotations' para explicar comportamientos invisibles, la creación de prototipos clicables en escala de grises para tests de concepto y la preparación de la librería de estilos estructurales para el equipo de UI) ...

---

## Referencia ampliada

Para ejemplos extendidos, métricas y notas, consulta [`reference.md`](reference.md) (cárgalo solo cuando necesites ese detalle).
