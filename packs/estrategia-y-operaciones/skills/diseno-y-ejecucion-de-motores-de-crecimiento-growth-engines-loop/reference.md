# Referencia ampliada — Diseño y Ejecución de Motores de Crecimiento (Growth Engines & Loops)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de aceleración del crecimiento.*

1.  **Trigger:** Un usuario completa una acción de alto valor en el producto (Ej: Finaliza su primer proyecto, realiza una compra).
2.  **Nodo de Evaluación de Potencial Viral:** El sistema analiza si el perfil del usuario es propenso a compartir y si el contexto es ideal (Momento de felicidad).
3.  **Nodo de Disparo de Incentivo Dinámico:** IA genera una oferta única o un "premio" que solo se desbloquea invitando o realizando una acción que alimente el bucle.
4.  **Nodo de Monitorización de Conversión Viral:** Se rastrea la procedencia de los nuevos usuarios para atribuirlos al bucle y optimizar los disparadores.
5.  **Output:** Incremento del coeficiente de viralidad; el sistema se auto-optimiza basándose en qué incentivos funcionan mejor para cada segmento.

---

## 7. Ejemplo Práctico: App de Envío de Archivos (Dropbox/WeTransfer Style)
**Reto:** El coste de captar usuarios con anuncios era más caro de lo que pagaban por el servicio.
**Acción v2.0:** Se implementó un bucle de adquisición: Cada vez que un usuario compartía un enlace con un no-usuario, este último veía una invitación a crear su cuenta para "responder de forma rápida".
**Resultado:** El 40% de los receptores de archivos se convertían en usuarios. El CAC bajó a casi cero y la empresa creció un 2000% en 18 meses sin inversión publicitaria masiva.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
