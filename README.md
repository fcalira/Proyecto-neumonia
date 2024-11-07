# Proyecto de Clasificación de Imágenes Médicas: Detección de Neumonía

Este proyecto tiene como objetivo construir un modelo de inteligencia artificial capaz de detectar neumonía en radiografías de tórax utilizando redes neuronales convolucionales (CNN). 
La detección temprana de la neumonía es crucial para un tratamiento adecuado y oportuno, y la inteligencia artificial puede automatizar y acelerar este proceso.

## Descripción del Proyecto

La neumonía es una enfermedad respiratoria grave que afecta a millones de personas alrededor del mundo. 
El diagnóstico temprano es crucial para su tratamiento, y las radiografías de tórax son una de las herramientas más utilizadas para su detección. 
Sin embargo, el análisis de estas imágenes requiere de personal médico capacitado, lo cual puede hacer que el proceso sea lento y costoso.

La solución propuesta en este proyecto es usar redes neuronales convolucionales (CNN) para clasificar automáticamente las radiografías en dos categorías:
- **Normal**: Radiografías de personas sin neumonía.
- **Pneumonia**: Radiografías de personas con neumonía.

### Proceso del Proyecto

1. **Recopilación de Datos**: Se utilizaron imágenes de radiografías de tórax, cada una etiquetada como "Normal" o "Pneumonía".
2. **Preparación de los Datos**: Las imágenes fueron redimensionadas y preprocesadas para que pudieran ser utilizadas por el modelo de IA.
3. **Entrenamiento del Modelo**: Se entrenó un modelo de red neuronal convolucional (CNN) para detectar patrones en las imágenes que indicaran la presencia de neumonía.
4. **Evaluación del Modelo**: El modelo fue evaluado en un conjunto de validación para verificar su rendimiento.
5. **Despliegue del Modelo**: El modelo entrenado se desplegó en una API web, lo que permite realizar predicciones en tiempo real sobre imágenes de radiografías de tórax.

### ¿Cómo Funciona el Modelo?

- **Redes Neuronales Convolucionales (CNN)**:
  Las CNN son un tipo especial de redes neuronales diseñadas para trabajar con imágenes.
  Pueden detectar características como bordes, texturas y patrones complejos, lo que las hace ideales para tareas de clasificación de imágenes.
- **Entrenamiento Supervisado**:
  El modelo fue entrenado usando imágenes etiquetadas como "Normal" o "Pneumonía", lo que permitió que aprendiera a hacer predicciones precisas.
- **Evaluación con Validación Cruzada**:
  Para asegurarnos de que el modelo generalizara bien a nuevos datos, se utilizó un conjunto de validación para evaluar su rendimiento en imágenes no vistas durante el entrenamiento.

### API Web

Para interactuar con el modelo de forma práctica, se creó una **API web**. 
Esto permite que cualquier usuario cargue una imagen de radiografía de tórax y reciba una predicción sobre si la imagen muestra "Normal" o "Pneumonía".

- **URL de la API**: [https://475b-34-169-63-196.ngrok-free.app/](https://475b-34-169-63-196.ngrok-free.app/)

### Archivos del Proyecto

- **`modelo_entrenado.keras`**: El modelo entrenado para la clasificación de neumonía.
- **`notebook_colab.ipynb`**: El archivo de Google Colab con el código que incluye el preprocesamiento de datos, entrenamiento y evaluación del modelo.
- **`presentación.pptx`**: La presentación que describe el problema, la solución, y los resultados obtenidos.
