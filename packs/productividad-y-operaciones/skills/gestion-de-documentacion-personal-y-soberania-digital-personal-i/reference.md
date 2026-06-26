# Referencia ampliada — Gestión de Documentación Personal y Soberanía Digital (Personal Information Architecture)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Auditoría de Superficie y Diseño de la Bóveda Maestra
**Objetivo:** Identificar vulnerabilidades y centralizar la gestión de accesos.
1.  **Inventario de Identidad Digital:** IA ayuda a rastrear todas las cuentas asociadas al email del usuario para identificar servicios olvidados o brechas de seguridad.
2.  **Configuración de la 'Fortaleza' Digital:** Instalación de gestor de contraseñas y activación de 2FA basado en app o hardware (No SMS).

**Prompt Maestro de Soberanía Digital (Digital Archivist):**
```text
Actúa como un Senior Security Consultant y Experto en Arquitectura de Información Personal. Diseña el sistema de gestión documental para: [USUARIO/FAMILIA]. 
1. Arquitectura de Carpetas Maestra: Propón una estructura de 5 áreas de vida principales y subniveles lógicos para que cualquier documento se guarde en menos de 5 segundos. 
2. Protocolo de Blindaje de Cuentas: Diseña el checklist de seguridad para las 4 cuentas críticas (Email, Banco, Cloud, Gov) incluyendo MFA y rotación de claves. 
3. Estrategia de Respaldo 3-2-1: Especifica qué servicios cloud y qué hardware local (Ej: NAS/SSD) usaremos para garantizar que los datos nunca se pierdan. 
4. Guía de Digitalización (Paperless): Define el flujo desde que llega un papel por correo físico hasta que está indexado y destruido de forma segura. 
5. Diseño del 'Bote de Rescate' (Legacy Kit): ¿Cómo y dónde guardaremos las instrucciones maestras para que los herederos accedan a la información en caso de emergencia?
```

### Fase 2: Ejecución, Limpieza Profunda y Mantenimiento de la Paz Digital
... (Expansión técnica sobre el uso de la técnica de 'Inbox Zero' aplicada a archivos, la implementación de un proceso de 'Encryption-at-rest' para archivos locales sensibles, y la monitorización de las 'Alertas de Brechas de Seguridad' (HaveIBeenPwned) para reaccionar antes que los atacantes) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de seguridad total.*

1.  **Trigger:** Recepción de un nuevo documento (Digital o Físico) o inicio de una sesión de auditoría de seguridad programada.
2.  **Nodo de Clasificación y Cifrado:** El sistema ayuda a renombrar el archivo según el estándar y sugiere la ubicación segura (Cifrada si es sensible).
3.  **Nodo de Sincronización y Backup Multicapa:** El documento se replica automáticamente en la nube de trabajo, el disco de respaldo local y la copia fría (Cold Storage).
4.  **Nodo de Auditoría de Identidad:** El sistema verifica que las contraseñas no han sido expuestas y que los accesos MFA están funcionando correctamente.
5.  **Output:** Vida digital ordenada y blindada; documentos críticos localizables en 3 clicks; backups validados; usuario con paz mental absoluta sobre su información.

---

## 7. Ejemplo Práctico: El Caso de 'Eduardo Digital'
**Reto:** Eduardo perdió su portátil y con él todas las fotos de su hijo, las escrituras de su casa escaneadas y las claves de sus cuentas bancarias que tenía en un Excel. Pasó 3 meses de pesadilla intentando recuperar sus accesos y el dolor de perder sus fotos fue incalculable.
**Acción v2.0:** Eduardo implementó Skill 258 tras el desastre. Ahora usa Bitwarden con Yubikey, tiene sus fotos en una nube cifrada y un backup físico en casa de sus padres, y cada documento nuevo que recibe lo escanea con el móvil y lo guarda por fecha.
**Resultado:** Seis meses después, Eduardo borró por error una carpeta financiera crítica. Tardó exactamente 45 segundos en recuperarla desde su backup en la nube. Duerme tranquilo sabiendo que, pase lo que pase con sus dispositivos físicos, su vida digital está a salvo y perfectamente organizada.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
