# Proyecto de Clasificación de Gatos y Perros

Este proyecto utiliza TensorFlow y Keras para crear un modelo de clasificación de imágenes de gatos y perros. El objetivo es entrenar un modelo que pueda distinguir entre imágenes de gatos y perros.

## Descripción del Proyecto

### Descarga de Datos

Para este proyecto, se utilizó un conjunto de datos que contiene imágenes de gatos y perros. Estas imágenes se descargaron y descomprimieron utilizando el siguiente código:

```python
!wget https://cdn.freecodecamp.org/project-data/cats-and-dogs/cats_and_dogs.zip
!unzip cats_and_dogs.zip
```
### Estructura de Carpetas
El conjunto de datos se organiza en tres directorios: train, validation y test, cada uno conteniendo imágenes de gatos y perros.

```
PATH = '/content/cats_and_dogs/'
train_dir = '/content/cats_and_dogs/train/'
validation_dir = '/content/cats_and_dogs/validation/'
test_dir = '/content/cats_and_dogs/test/'
```

### Preprocesamiento de Datos
Se realizaron operaciones de preprocesamiento en las imágenes, incluyendo la normalización y redimensionamiento a un tamaño específico.

```
width = 300
height = 300
size = (300, 300)
```

### Creación del Conjunto de Datos
Se crearon conjuntos de datos (x_data y y_data) a partir de las imágenes de entrenamiento. Cada imagen se redimensionó y se asignó una etiqueta correspondiente (0 para gatos y 1 para perros).

### Creación del Modelo
Se construyó un modelo de red neuronal convolucional (CNN) utilizando TensorFlow y Keras.

### Entrenamiento del Modelo
El modelo se entrenó con los datos de entrenamiento durante 100 épocas.

### Guardar y Cargar el Modelo
El modelo entrenado se guardó en un archivo llamado 'ic_model.keras' y se cargó para su uso posterior.

### Prueba del Modelo
Se realizó una prueba del modelo utilizando una imagen de prueba. La predicción se realizó sobre la imagen y se mostró el resultado (gato o perro).

### Conclusiones
Este proyecto implementa un desarrollo básico de un modelo de clasificación de imágenes utilizando TensorFlow y Keras. Puede ajustarse y mejorar según las necesidades específicas del usuario.
