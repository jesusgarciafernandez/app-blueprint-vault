# Referencia ampliada — Estrategia de Producto Basada en Inteligencia Artificial (AI-First Product Strategy)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de ejecución inteligente.*

1.  **Trigger:** El usuario solicita una tarea compleja mediante lenguaje natural o el sistema detecta una oportunidad de asistencia proactiva.
2.  **Nodo de Orquestación de Agentes:** El sistema selecciona el modelo o prompt específico según la intención detectada.
3.  **Nodo de Inyección de Contexto (RAG):** Se recuperan los datos relevantes del usuario o del negocio para que la respuesta sea precisa y útil.
4.  **Nodo de Validación y Formateo:** Se comprueba el output contra los filtros de seguridad y se adapta el formato (JSON, Markdown, HTML) para la interfaz.
5.  **Output:** Tarea completada con éxito; el sistema pide feedback al usuario para seguir refinando el modelo en el futuro.

---

## 7. Ejemplo Práctico: App de Gestión de Proyectos para Construcción
**Reto:** Los jefes de obra no tienen tiempo para escribir informes diarios. Solo mandan fotos y notas de audio desordenadas por WhatsApp.
**Acción v2.0:** Se implementó una capa de IA que transcribe los audios, analiza las fotos para detectar progresos o riesgos y genera automáticamente el informe diario estructurado.
**Resultado:** Los informes pasaron de tardar 2 horas de oficina a 0 minutos de escritorio. La visibilidad para el cliente final mejoró un 100% y la App se convirtió en líder de mercado por su facilidad de uso radical.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
