# Referencia ampliada — Generador de Encuestas Inteligentes (Dynamic Survey Engine)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Objetivos y Diseño del Árbol Lógico
**Objetivo:** Obtener la máxima información con el mínimo esfuerzo del usuario.
1.  **Definición del 'Core Insight':** IA ayuda a refinar las preguntas para que sean claras, no sesgadas y directas al grano.
2.  **Mapeo de Saltos Lógicos (Logic Tree):** Diseño visual o textual del árbol de decisiones (Ej: Si pregunta 1 == 'A', saltar a página 4).

**Prompt Maestro de Diseño de Encuestas (Insight Architect):**
```text
Actúa como un Senior UX Research y Experto en Conversión de Leads. Diseña el flujo de la encuesta inteligente para: [PROPÓSITO_ENCUESTA]. 
1. Estructura de Captación: Define las 3 preguntas de cualificación inicial que segmentarán el flujo del usuario. 
2. Diseño de Lógica de Salto (Logic Jumps): Describe las reglas condicionales (Ej: Si el usuario es 'SaaS', preguntar por su MRR; si es 'E-commerce', preguntar por su plataforma de venta). 
3. Redacción de Preguntas Empáticas: Escribe las preguntas usando un tono conversacional que reduzca la fricción y aumente la veracidad de la respuesta. 
4. Estrategia de Cierre y 'Call to Action': Diseña la pantalla final personalizada según el perfil detectado (Ej: Ofrecer una demo personalizada o un recurso descargable específico). 
5. Integración de Datos: Define qué metadatos (Ej: Referrer, Tiempo en completar, Dispositivo) recolectaremos de forma invisible para enriquecer el análisis.
```

### Fase 2: Ejecución, Programación y Análisis de Conversión
... (Expansión técnica sobre el uso de la técnica de 'Hidden Fields' para pasar contexto de usuario sin preguntar, la implementación de un proceso de 'Drop-off Analysis' para detectar en qué pregunta abandona la gente, y la monitorización de la 'Tasa de Completitud' para optimizar la longitud de la encuesta dinámicamente) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de escucha activa.*

1.  **Trigger:** El usuario accede al enlace de la encuesta o ésta se le presenta tras una acción específica en la web (Ej: 2 minutos navegando).
2.  **Nodo de Personalización de Bienvenida:** El sistema carga los datos conocidos del usuario y adapta el mensaje inicial para que sea personal.
3.  **Nodo de Navegación Dinámica:** El motor de lógica evalúa cada respuesta y decide qué pregunta o pantalla mostrar a continuación en milisegundos.
4.  **Nodo de Disparo Post-Respuesta:** Al finalizar, el sistema envía los datos a las herramientas de negocio y genera un resumen inmediato para el usuario si es necesario.
5.  **Output:** Datos cualitativos limpios y segmentados en el CRM; experiencia de usuario satisfactoria; disparadores de marketing o ventas activados automáticamente.

---

## 7. Ejemplo Práctico: Agencia de Seguros 'ProtecciónTotal'
**Reto:** 'ProtecciónTotal' tenía un formulario de solicitud de presupuesto de 40 preguntas que casi nadie terminaba. Sus comerciales perdían mucho tiempo llamando a gente que no era su cliente ideal.
**Acción v2.0:** Implementaron Skill 245. Crearon una encuesta inteligente que primero preguntaba "¿Qué quieres proteger?". Según la respuesta (Casa, Coche, Vida), el resto de la encuesta cambiaba totalmente.
**Resultado:** La tasa de formularios completados subió un 400%. Los comerciales ahora solo reciben solicitudes de gente que ya ha sido pre-cualificada por la encuesta, y cierran ventas el doble de rápido porque ya tienen toda la información necesaria segmentada.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
