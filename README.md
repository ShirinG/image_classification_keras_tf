# Workshop material for ML Summit 2018

## Bildklassifikation leicht gemacht – mit Keras und TensorFlow

Tuesday, 2. October 2018 | 10:00 - 13:00

Lange Zeit galt die automatische Erkennung von Objekten, Menschen und Szenen auf Bildern durch Computer als unmöglich. Die Komplexität schien schlicht zu groß, um sie einem Algorithmus programmatisch beibringen zu können. Doch Neuronale Netze haben dies drastisch verändert! Inzwischen ist Bilderkennung ist ein weit verbreitetes Anwendungsgebiet von Maschinellem Lernen. Häufig werden dafür sogenannte “Convolutional Neuronal Networks”, oder “ConvNets” verwendet. In diesem Workshop werde ich zeigen, wie einfach es ist, solch ein Neuronales Netz selber zu bauen. Dafür werden wir Keras und TensorFlow verwenden. Wir werden zunächst ein komplettes Netz selber trainieren: vom Einlesen der Bilder, über das Definieren des Netzes, hin zum Evaluieren auf Testbildern. Anschließend gucken wir uns an, wie man mit Transfer Learning und vortrainierten Netzen auch mit wenigen eigenen Bildern schnell Erfolge sehen kann. Im letzten Teil des Workshops soll es dann darum gehen, wie wir diese Bilderkennungsmodelle besser verstehen können – zum Beispiel indem wir die Knoten in Zwischenschichten visualisieren; so können wir Muster und für die Klassifikation wichtige Bildbereiche finden und die Klassifikation durch das Modell nachvollziehen.
Installationshinweise: Wir werden mit Python3 in Google Collaboratory arbeiten.

## Installation / Docker

-  Docker installieren

## Jupyterlab starten

Docker image enthält:
[https://github.com/codecentric/from-keras-to-production-baseimage](https://github.com/codecentric/from-keras-to-production-baseimage)

- Datensatz (fruits)
- Vortrainierte Netze (VGG16, ResNet50, Xception)
- Keras
- TensorFlow
- Python3
- benötigte Pythonpakete

```bash
docker pull codecentric/from-keras-to-production-baseimage
```

## Run on Mac & Linux

```bash
docker run -p 8888:8888 -v $(pwd)/notebooks:/keras2production/notebooks codecentric/from-keras-to-production-baseimage
```
## Run on Windows

```bash
docker run -p 8888:8888 -v %cd%/notebooks:/keras2production/notebooks codecentric/from-keras-to-production-baseimage
```

