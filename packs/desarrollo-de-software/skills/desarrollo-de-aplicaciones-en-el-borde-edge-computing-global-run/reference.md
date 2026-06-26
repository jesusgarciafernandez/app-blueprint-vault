# Referencia ampliada — Desarrollo de Aplicaciones en el Borde (Edge Computing & Global Runtimes)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de proximidad instantánea.*

1.  **Trigger:** Petición HTTP entrante desde el navegador del usuario hacia el dominio de la aplicación.
2.  **Nodo de Intercepción en el Borde:** El nodo de red más cercano al usuario captura la petición (0.5ms-20ms de distancia).
3.  **Nodo de Ejecución de Lógica Edge:** Se ejecuta la función serverless (Auth/Redirección/Caché) sin arrancar servidores pesados.
4.  **Nodo de Respuesta Instantánea o Proxy:** El sistema devuelve los datos directamente si están en caché o modifica la petición antes de enviarla al origen central.
5.  **Output:** Usuario recibe la web personalizada e instantánea; telemetría de rendimiento enviada al dashboard central de infraestructura.

---

## 7. Ejemplo Práctico: Periódico Global 'InstantNews'
**Reto:** Los usuarios de Australia tardaban 4 segundos en ver la portada porque los servidores estaban en Londres, y la publicidad se cargaba con retraso.
**Acción v2.0:** Implementaron Edge Computing (Skill 233) con Cloudflare Workers. Movieron la lógica de selección de noticias y la inyección de banners al borde.
**Resultado:** El tiempo de carga en Australia bajó a 300ms. Al personalizar la portada en el borde según el interés del lector, el tiempo de permanencia en la web subió un 45%.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
