# Workshop material for Image Classification with Python, Keras and TensorFlow

## Installation / Docker

-  Docker installieren

## Jupyterlab starten

Docker image [https://github.com/codecentric/from-keras-to-production-baseimage](https://github.com/codecentric/from-keras-to-production-baseimage) enthält:

- Datensatz (fruits)
- Vortrainierte Netze (VGG16, ResNet50, Xception)
- Keras
- TensorFlow
- Python3
- benötigte Pythonpakete

**BEWARE: das Image ist sehr groß, enthält dafür aber alles, was zum selber ausprobieren benötigt wird!**

```bash
docker pull codecentric/from-keras-to-production-baseimage
```

## Run on Mac & Linux

```bash
docker run -p 8888:8888 -v $(pwd)/notebooks:/keras2production/notebooks codecentric/from-keras-to-production-baseimage
```
## Run on Windows

- %cd% oder absoluten Pfad zum Ordner "notebooks"

```bash
docker run -p 8888:8888 -v %cd%/notebooks:/keras2production/notebooks codecentric/from-keras-to-production-baseimage
```

