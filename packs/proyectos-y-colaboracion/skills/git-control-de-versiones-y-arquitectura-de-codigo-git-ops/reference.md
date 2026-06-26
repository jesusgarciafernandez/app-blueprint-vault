# Referencia ampliada — Git, Control de Versiones y Arquitectura de Código (Git Ops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de versiones operativa.*

1.  **Trigger:** Guardado de cambios local, creación de una nueva rama, o solicitud de fusión (Pull Request).
2.  **Nodo de Pre-Commit (Hooks):** La IA revisa localmente que el código cumple con los estándares de estilo antes de permitir el 'commit'.
3.  **Nodo de Verificación de Integridad (GitHub Action):** Se corren los tests automáticos al subir al servidor remoto.
4.  **Nodo de Alerta de Conlicto Predictivo:** El sistema avisa: "Cuidado, estás modificando el mismo archivo que el desarrollador B. Sincroniza pronto para no tener conflictos pesados".
5.  **Output:** Código siempre respaldado, limpio y desplegable; historial de cambios transparente; equipo trabajando en perfecta sintonía.

---

## 7. Ejemplo Práctico: El caso de 'AppScale'
**Reto:** 'AppScale' era una aplicación de finanzas. Tenían a 3 programadores trabajando juntos. Uno de ellos, por error, borró la función de pago y subió el cambio a la carpeta compartida de Dropbox que usaban. El desastre fue total: no sabían quién lo había hecho ni tenían copia de seguridad de la versión anterior que funcionaba. Estuvieron parados 3 días perdiendo 50.000€.
**Acción v2.0:** Implementaron Skill 355. Migraron todo a GitHub. Configuraron una rama 'main' protegida.
**Resultado:** Dos semanas después, otro desarrollador subió un error por accidente. Esta vez, el sistema de CI/CD bloqueó la subida antes de que afectara a nadie. El CEO pudo ver en el historial exactamente qué se había roto. Hicieron un `git revert` en 2 minutos y la empresa siguió facturando sin que el usuario notara nada. 'AppScale' ahora es una empresa de software profesional.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
