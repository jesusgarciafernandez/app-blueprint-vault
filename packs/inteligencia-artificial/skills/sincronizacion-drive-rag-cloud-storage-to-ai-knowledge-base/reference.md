# Referencia ampliada — Sincronización Drive-RAG (Cloud Storage to AI Knowledge Base)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Origen y Configuración de Acceso
**Objetivo:** Definir qué carpetas son "Mente" y establecer la conexión segura.
1.  **Mapeo de Estructura de Drive:** IA ayuda a identificar las carpetas raíz que contienen información valiosa y a definir reglas de exclusión (Ej: ignorar archivos temporales o copias).
2.  **Configuración del Webhook/Trigger:** Establecimiento de la frecuencia de sincronización (Ej: Cada 15 min o tras cada edición).

**Prompt Maestro de Sincronización Drive-RAG:**
```text
Actúa como un Senior Cloud Engineer y Experto en Pipelines de Datos para IA. Diseña el sistema de sincronización entre [CARPETAS_DRIVE] y [VECTOR_DB]. 
1. Estructura de Conexión: Define cómo autenticaremos el sistema (Service Account vs OAuth) y qué scopes de permisos son los mínimos necesarios por seguridad. 
2. Pipeline de Procesamiento: Describe los pasos para extraer texto de archivos .gdoc y .pdf, asegurando que los metadatos de Drive (Nombre de archivo, Autor, URL) se guarden con el vector. 
3. Lógica de 'Delta Sync': Diseña el algoritmo para identificar si un archivo es nuevo, ha sido modificado o ha sido borrado, para reflejar exactamente ese estado en la Knowledge Base. 
4. Gestión de Errores y Límites: ¿Cómo manejaremos los 'Rate Limits' de la API de Google y qué hacer si un documento es demasiado pesado o está corrupto? 
5. Protocolo de Notificación: Crea una alerta automática (Ej: Slack/Email) que informe al humano cuando se han indexado nuevos conocimientos con éxito.
```

### Fase 2: Ejecución, Limpieza de Datos y Validación
... (Expansión técnica sobre el uso de la técnica de 'Semantic Chunking' aplicada a documentos de Drive, la implementación de un sistema de 'De-duplicación' para evitar recuerdos repetidos y la monitorización de la latencia entre que un archivo se guarda en la nube y está disponible para la IA en el chat) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de sincronización de conocimiento fluida.*

1.  **Trigger:** Evento de "Nuevo Archivo" o "Modificación" detectado en una carpeta monitorizada de Google Drive.
2.  **Nodo de Descarga y Conversión:** El sistema baja el archivo y lo transforma en texto plano estructurado (Markdown/JSON).
3.  **Nodo de Fragmentación (Chunking) e Indexación:** Se divide el texto, se generan los embeddings y se suben a la Vector DB actualizando los punteros de metadatos.
4.  **Nodo de Verificación de Integridad:** Un proceso automático lanza una pregunta de prueba sobre el nuevo documento para asegurar que es "recuperable" con éxito.
5.  **Output:** Knowledge Base actualizada; la IA responde basado en la información más reciente; log de sincronización disponible para el administrador.

---

## 7. Ejemplo Práctico: Despacho de Abogados 'LexCloud'
**Reto:** Los abogados redactaban escritos en Google Drive pero cuando usaban la IA para consultas, esta les citaba leyes de borradores antiguos porque no se habían subido las versiones finales a la plataforma.
**Acción v2.0:** Implementaron Sincronización Drive-RAG (Skill 228). La IA monitoriza la carpeta "Casos_Finalizados".
**Resultado:** En cuanto un abogado guarda el PDF final en Drive, la IA lo indexa en 60 segundos. Todo el despacho tiene ahora un consultor virtual que conoce cada precedente ganado por la firma sin que nadie tenga que subir un solo archivo manualmente.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
