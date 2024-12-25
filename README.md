# Procesamiento de imágenes con YOLO y visión por computadora

Este proyecto utiliza el modelo **YOLO (You Only Look Once)** para procesar imágenes y detectar objetos en ellas. El código está dividido en tres fases principales: creación de una carpeta para almacenar resultados, procesamiento de la imagen y descarga de los resultados en un archivo ZIP. Desarrollado or José R. Leonett para la comunidad de 

![image](https://lh3.googleusercontent.com/d/1dWjYPUS0MHsnFEbMmfQO7kTFJgOP0hnR)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jrleonett/visioncomputacional/blob/main/visioncomputacional.ipynb)

---

## Tipos de objetos que YOLO puede identificar.
El modelo YOLO utilizado en este proyecto está entrenado con el conjunto de datos **COCO (Common Objects in Context)**, que incluye 80 clases de objetos comunes. Algunos de los objetos que YOLO puede identificar son:

- **Personas**: `person`
- **Vehículos**: `car`, `bus`, `truck`, `motorcycle`, `bicycle`
- **Animales**: `dog`, `cat`, `horse`, `elephant`, `zebra`
- **Objetos de uso diario**: `chair`, `table`, `book`, `cell phone`, `laptop`
- **Alimentos**: `banana`, `apple`, `orange`, `pizza`, `sandwich`
- **Deportes**: `sports ball`, `frisbee`, `skateboard`, `kite`, `baseball bat`

Para ver la lista completa de objetos, consulta el archivo `coco.names`.

---

## Fase 1: Creación de la carpeta "EVIDENCIA".
En esta fase, se crea una carpeta llamada **"EVIDENCIA"** en el directorio actual. Esta carpeta se utilizará para almacenar los resultados del procesamiento de la imagen.

---

## Fase 2: Procesamiento de la imagen y detección de objetos.
1. **Carga del modelo YOLO**: Se carga el modelo preentrenado **YOLO** utilizando los archivos `yolov3.weights`, `yolov3.cfg` y `coco.names`.
2. **Subida de la imagen**: El usuario sube una imagen desde su computadora a Google Colab.
3. **Detección de objetos**: La imagen se procesa utilizando el modelo YOLO para identificar objetos.
4. **Dibujo de detecciones**: Los objetos detectados se marcan en la imagen con cuadros delimitadores y etiquetas.
5. **Guardado de resultados**: La imagen procesada se guarda en la carpeta **"EVIDENCIA"**.

---

## Fase 3: Creación y descarga del archivo ZIP.
1. **Creación del archivo ZIP**: Se comprime la carpeta **"EVIDENCIA"** en un archivo ZIP.
2. **Descarga del archivo**: El archivo ZIP se descarga automáticamente a la computadora del usuario.

---

## Requisitos.
Para ejecutar este código, es necesario tener los siguientes archivos en el entorno de Google Colab:
- `yolov3.weights`: Pesos del modelo YOLO.
- `yolov3.cfg`: Configuración del modelo YOLO.
- `coco.names`: Archivo que contiene los nombres de las clases que YOLO puede detectar.

---

## Notas.
- **Ubicación de los archivos**: Asegúrate de que los archivos de YOLO estén en el mismo directorio que tu notebook de Colab.
- **Ajustes de detección**: Puedes modificar los umbrales de confianza (`conf_threshold`) y el umbral de NMS (`nms_threshold`) para mejorar la precisión de la detección.

---

# Cómo citar este trabajo.
Usa la siguiente entrada BibTeX si utilizas este trabajo en tu investigación:
```bash
@article{joséRLeonett,
  title={Análisis FFT y Espectrográfico de audios},
  author={José R. Leonett},
  year={2024}
}
```

**Licencia.**
- Este proyecto está bajo la licencia MIT. Consulta el archivo LICENSE para más detalles.


