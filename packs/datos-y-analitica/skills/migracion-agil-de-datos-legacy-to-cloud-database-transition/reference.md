# Referencia ampliada — Migración Ágil de Datos (Legacy to Cloud Database Transition)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de transporte de datos.*

1.  **Trigger:** Carga de un nuevo archivo .accdb o .xlsx en una carpeta de vigilancia (Watch folder) o activación programada.
2.  **Nodo de Extracción y Parsing:** El sistema lee los datos crudos y los carga en una área temporal de "staging".
3.  **Nodo de Transformación por IA:** Aplicación de reglas de limpieza y validación semántica de los registros.
4.  **Nodo de Carga en SQL Cloud:** El sistema inserta o actualiza los datos en la base de datos de producción asegurando la integridad.
5.  **Output:** Base de datos Cloud actualizada y sincronizada; reporte de errores enviado al administrador si algún registro fue rechazado por validación.

---

## 7. Ejemplo Práctico: Empresa de Distribución 'LocalLogs'
**Reto:** Gestionaban 50.000 pedidos en una base de datos Access que se corrompía cada semana. Solo una persona podía editarla a la vez.
**Acción v2.0:** Migraron a Supabase (PostgreSQL Cloud). Automatizaron un script en Python que limpió los datos duplicados y los cargó en 10 minutos.
**Resultado:** Cero errores de corrupción. Ahora el equipo comercial (15 personas) puede consultar y editar pedidos simultáneamente desde sus móviles.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
