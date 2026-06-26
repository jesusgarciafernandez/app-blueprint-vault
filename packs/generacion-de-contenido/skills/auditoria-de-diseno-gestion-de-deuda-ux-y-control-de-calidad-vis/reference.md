# Referencia ampliada — Auditoría de Diseño, Gestión de Deuda UX y Control de Calidad Visual

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de control de calidad visual automatizada.*

1.  **Trigger:** El equipo de desarrollo realiza un 'Pull Request' con cambios en el CSS/Tokens de la interfaz.
2.  **Nodo de Comparativa de Regresión Visual:** IA compara píxel a píxel las nuevas pantallas con la versión maestra aprobada.
3.  **Nodo de Detección de Colores Fuera de Paleta:** El sistema avisa si se han introducido códigos HEX que no pertenecen al manual de marca.
4.  **Nodo de Generación de Alerta de Consistencia:** El sistema bloquea el despliegue si detecta que un componente core (ej. Botón Primary) ha cambiado su radio de borde sin autorización.
5.  **Output:** Informe automático de "Pase/Fallo" de diseño enviado al equipo de QA antes de salir a producción.

---

## 7. Ejemplo Práctico: Plataforma de Educación Online
**Reto:** Después de 3 años, la web tenía 5 tipos de menús diferentes y el 40% de los botones eran inaccesibles (poco contraste).
**Acción v2.0:** Se realizó una auditoría de diseño integral que identificó 200 puntos de inconsistencia. Se documentó todo en un muro de Miro y se priorizaron las correcciones de mayor impacto en la conversión.
**Resultado:** Al unificar el diseño bajo un solo estándar coherente, las llamadas a atención al cliente por "no encuentro el curso" bajaron un 30% y la velocidad de carga mejoró al limpiar el CSS redundante.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
