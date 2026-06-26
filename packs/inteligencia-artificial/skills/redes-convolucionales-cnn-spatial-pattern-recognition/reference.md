# Referencia ampliada — Redes Convolucionales (CNN & Spatial Pattern Recognition)

> Complemento de `SKILL.md`. Contiene el detalle extendido; cárgalo bajo demanda.

## 5. Instrucciones y Pasos Detallados (Protocolo Maestro)

### Fase 1: Arquitectura de la Red y Pipeline de Datos
**Objetivo:** Diseñar el "ojo digital" y su entrenamiento.
1.  **Selección del Backbone:** IA ayuda a elegir la red base (Ej: ResNet50 para precisión vs MobileNetV3 para velocidad) según el hardware de despliegue.
2.  **Configuración de 'Aumento de Datos' (Data Augmentation):** Diseño de giros, recortes y cambios de brillo sintéticos para que la IA aprenda a reconocer el objeto en cualquier condición.

**Prompt Maestro de Redes Convolucionales:**
```text
Actúa como un Senior Computer Vision Architect y Experto en Deep Learning. Diseña el sistema de visión CNN para el reto: [DESCRIPCIÓN_RETO_VISUAL]. 
1. Estructura de Capas: Define la jerarquía de convoluciones y si usaremos 'Residual Connections' o 'Squeeze-and-Excitation' para mejorar el flujo de información. 
2. Prep-procesado y Augmentation: Propón 5 técnicas de transformación de imágenes para evitar el sobreajuste y que el modelo sea robusto ante [CONDICIONES_AMBIENTALES]. 
3. Selección de 'Loss Function': Define si usaremos 'Cross-Entropy' para clasificación pura o 'Focal Loss' si tenemos un problema de desequilibrio de clases (objetos raros). 
4. Estrategia de Inferencia: ¿Cómo optimizaremos el modelo resultante (Ej: Cuantización INT8) para que procese al menos 30 frames por segundo en una [DISPOSITIVO_DESTINO]? 
5. Protocolo de Validación Visual: Diseña un test de 'Heatmaps' (Grad-CAM) para visualizar qué píxeles está mirando la IA antes de decidir y asegurar que no se guía por ruido de fondo.
```

### Fase 2: Ejecución, Depuración de Gradientes y Evaluación Final
... (Expansión técnica sobre el uso de la técnica de 'Feature Map Visualization' para entender qué está aprendiendo cada capa, la implementación de un proceso de 'Object Detection' con cajas delimitadoras (Bounding boxes) y la monitorización de la 'Precisión-Recall' para asegurar que el modelo visual es fiable y seguro para su uso en entornos críticos) ...

---

## 6. Arquitectura de Automatización Lógica (Agnostic Flow)
*Lógica de percepción espacial.*

1.  **Trigger:** Entrada de una trama de video o imagen (archivo o streaming) al sistema.
2.  **Nodo de Pre-procesado y Reescalado:** IA ajusta la resolución y normaliza los colores para adaptarlos a la entrada exacta de la red neuronal.
3.  **Nodo de Inferencia Convolucional:** La red recorre la imagen en capas, detectando patrones y generando una representación abstracta de alto nivel.
4.  **Nodo de Clasificación/Detección:** La capa final (Head) traduce los patrones en etiquetas (ej: "Gato: 98%") o coordenadas de objetos.
5.  **Output:** Imagen procesada con metadatos de detección; alerta activada si se identifica un objeto crítico definido por el humano.

---

## 7. Ejemplo Práctico: Seguridad Vial 'BlindSpotAI'
**Reto:** Los camiones tienen puntos ciegos donde los retrovisores no llegan. Los sensores clásicos de proximidad pitan por cualquier cosa (farolas, lluvia), causando que el conductor los ignore.
**Acción v2.0:** Implementaron Redes Convolucionales (Skill 229). Entrenaron una CNN para identificar específicamente "siluetas humanas y bicicletas" en tiempo real desde cámaras laterales.
**Resultado:** El sistema solo avisa si hay un humano en peligro, ignorando objetos inanimados. Los accidentes de giro se redujeron un 80% en la flota de pruebas.

---
**Autor:** Jesús García Fernández  
**Licencia:** CC BY-NC-SA 4.0
