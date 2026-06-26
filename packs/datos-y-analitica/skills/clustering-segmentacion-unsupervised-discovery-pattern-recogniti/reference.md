# Referencia ampliada — Clustering & Segmentación (Unsupervised Discovery & Pattern Recognition)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de segmentación automática.*

1.  **Trigger:** Ingesta periódica de datos de actividad de clientes o inventario.
2.  **Nodo de Escalado y Transformación:** El sistema normaliza los datos automáticamente para que tengan media 0 y varianza 1.
3.  **Nodo de Agrupación por IA:** El algoritmo K-means asigna cada nuevo registro al cluster correspondiente en milisegundos.
4.  **Nodo de Etiquetado de Negocio:** El sistema añade el nombre del segmento al perfil del cliente (Ej: "Segmento: VIP", "Segmento: En riesgo").
5.  **Output:** Clientes segmentados dinámicamente; las campañas de marketing automatizadas se activan según el grupo asignado.

---

## 7. Ejemplo Práctico: App de Fitness 'LifeActive'
**Reto:** Trataban a todos los usuarios igual. Los "Principiantes" se agobiaban con el contenido avanzado y los "Expertos" se aburrían.
**Acción v2.0:** Aplicaron clustering basándose en la intensidad de los entrenamientos y la frecuencia de login. La IA detectó 4 grupos claros.
**Resultado:** Personalizaron el feed de noticias por segmento. La retención al segundo mes subió un 22% porque cada usuario recibía exactamente el nivel de desafío que necesitaba.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
