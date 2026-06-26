# Referencia ampliada — Modelado de Sistemas mediante Arquitectura C4 (Hierarchical System Visualization)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Contexto y Mapeo de Contenedores
**Objetivo:** Entender la posición del sistema en el mundo y su estructura interna.
1.  **Definición del Sistema (Nivel 1):** IA ayuda a identificar a los usuarios (Capa Humana) y a los sistemas externos con los que se integra la app core.
2.  **Identificación de Contenedores (Nivel 2):** Desglose de la arquitectura en piezas desplegables independientes (Web Apps, Databases, Mobile, Microservicios).

**Prompt Maestro de Modelado C4 (Visual Architect):**
```text
Actúa como un Principal Software Architect y Experto en Documentación Técnica. Modela el sistema [NOMBRE_SISTEMA] usando el modelo C4. 
1. Diagrama de Contexto (Nivel 1): Define a las personas (Personas) y los sistemas de software (Systems) que interactúan con el núcleo. ¿Quién lo usa y para qué? 
2. Diagrama de Contenedores (Nivel 2): Desglosa el sistema en sus unidades de despliegue principales. Especifica la tecnología (Ej: React, Go, MongoDB) y la responsabilidad técnica de cada 'caja'. 
3. Definición de Interconexiones: Para cada flecha de comunicación, especifica el protocolo (Ej: HTTPS/REST, gRPC, JDBC) y el flujo de información principal. 
4. Zoom a Componentes (Nivel 3): Selecciona el contenedor clave [CONTENEDOR_X] y describe los 3-5 componentes internos lógicos que lo forman. 
5. Formateo 'Architecture as Code': Genera el código Mermaid.js completo para los diagramas de Nivel 1 y Nivel 2, asegurando que sean visualizables en cualquier lector de markdown.
```

### Fase 2: Ejecución, Revisión de Componentes y Mantenimiento
... (Expansión técnica sobre el uso de la técnica de 'Dynamic Diagrams' para mostrar flujos de procesos específicos sobre el modelo estático, la implementación de un proceso de 'Review de Arquitectura' sincronizado con las PRs de código, y la monitorización de la 'Deuda Documental' para asegurar que los diagramas reflejen siempre el estado real de la producción) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de visibilidad sistémica.*

1.  **Trigger:** Inicio de diseño de una nueva funcionalidad arquitectónica o necesidad de documentar un módulo existente.
2.  **Nodo de Recolección de Datos Técnicos:** IA o el arquitecto analizan los límites del sistema, tecnologías implicadas y protocolos de red.
3.  **Nodo de Generación de Diagramas (DSL):** El sistema genera la descripción textual del modelo C4 (Mermaid/PlantUML) respetando la jerarquía de los 4 niveles.
4.  **Nodo de Validación de Coherencia:** El arquitecto verifica que las flechas y responsabilidades coincidan con la realidad del código y la estrategia del negocio.
5.  **Output:** Diagramas profesionales inyectados en el README o documentación del proyecto; modelo mental compartido y validado por el equipo técnico.

---

## 7. Ejemplo Práctico: Plataforma de Salud 'HealthConnect'
**Reto:** 'HealthConnect' tenía una arquitectura dispersa de microservicios. Cuando un nuevo desarrollador entraba, tardaba 3 semanas en entender cómo el login afectaba a la base de datos de pacientes crónicos. La documentación de texto era inútil por su longitud.
**Acción v2.0:** Implementaron Modelado C4 (Skill 238). Crearon una página de arquitectura con 3 niveles de zoom. Un diagrama de contexto para el negocio, uno de contenedores para DevOps y uno de componentes para los devs de backend.
**Resultado:** La curva de aprendizaje del nuevo talento bajó de 3 semanas a 2 días. Los ingenieros ahora consultan el diagrama de Nivel 2 antes de añadir cualquier nueva API para asegurar que no están duplicando responsabilidades en contenedores que no corresponden.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
