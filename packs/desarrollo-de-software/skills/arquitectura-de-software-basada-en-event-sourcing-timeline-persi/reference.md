# Referencia ampliada — Arquitectura de Software Basada en Event Sourcing (Timeline Persistence Management)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Modelado de Eventos de Dominio y Proyecciones
**Objetivo:** Capturar la intención del negocio en hechos inmutables.
1.  **Auditoría de Hechos Históricos:** IA ayuda a identificar qué acciones del usuario deben ser tratadas como eventos core que no pueden perderse ni modificarse.
2.  **Diseño de la Estrategia de Proyección:** Definición de cómo transformaremos el stream de eventos en vistas SQL/NoSQL rápidas para ser consultadas por el frontend.

**Prompt Maestro de Event Sourcing (Timeline Architect):**
```text
Actúa como un Principal Software Architect y Experto en Domain-Driven Design (DDD). Diseña la arquitectura de Event Sourcing para: [NOMBRE_SISTEMA]. 
1. Catálogo de Eventos: Identifica los 5 eventos fundamentales (Ej: RegistroIniciado, EmailVerificado, PerfilCompletado) y describe qué datos (Payload) llevará cada uno. 
2. Diseño del Event Store: Justifica la elección de la base de datos de eventos y define la clave de partición (Stream ID) para asegurar el orden de los mensajes. 
3. Implementación de CQRS: Diseña el flujo de 'Read Models' (Proyecciones). ¿Cómo mantendremos las tablas de consulta sincronizadas con el flujo de eventos? 
4. Estrategia de Retrocompatibilidad: ¿Cómo manejaremos un cambio en la estructura del evento [EVENTO_X] sin que el sistema falle al leer eventos de hace 2 años? 
5. Protocolo de 'Replay' de Datos: Define cómo reconstruiremos una base de datos de consulta completa desde cero si los datos de lectura se corrompen.
```

### Fase 2: Ejecución, Gestión de Snapshots y Evolución
... (Expansión técnica sobre el uso de la técnica de 'Snapshotting' para evitar leer millones de eventos al cargar una entidad, la implementación de un proceso de 'Event Upcasting' para transformar eventos antiguos a la nueva versión en tiempo de lectura, y la monitorización de la 'Latencia de Proyección' para asegurar que el usuario vea sus cambios reflejados en la interfaz casi instantáneamente) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de persistencia histórica.*

1.  **Trigger:** El usuario o un sistema externo intenta realizar una acción de cambio (Comando) sobre una entidad del negocio.
2.  **Nodo de Validación y Generación de Evento:** El sistema valida la lógica de negocio y, si es correcta, genera un objeto de 'Evento' con sello de tiempo y emisor.
3.  **Nodo de Persistencia Append-Only:** El evento se guarda de forma inmutable al final del stream correspondiente en el Event Store.
4.  **Nodo de Proyección Asíncrona:** Un proceso lee el nuevo evento y actualiza las bases de datos de lectura (SQL/Caché) para que el estado actual sea consultable.
5.  **Output:** Acción confirmada al usuario; el historial queda permanentemente enriquecido y disponible para auditorías o análisis de datos futuros.

---

## 7. Ejemplo Práctico: Aplicación de Cartera 'CriptoGuard'
**Reto:** Los usuarios de una app de criptomonedas se quejaban de que a veces desaparecían fondos de su saldo visual o que no entendían por qué tenían X cantidad tras varias compras y ventas.
**Acción v2.0:** Implementaron Event Sourcing (Skill 236). Dejaron de guardar el "Saldo Total" como una columna y pasaron a guardar cada 'Ingreso', 'Gasto', 'Intercambio' y 'Comisión' como eventos inmutables.
**Resultado:** La app ahora ofrece un botón de "Ver historial de saldo" que muestra la evolución exacta minuto a minuto. El equipo técnico puede reconstruir el saldo de cualquier usuario desde el día 1 en segundos, eliminando errores de redondeo y aumentando la confianza del usuario un 100%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
