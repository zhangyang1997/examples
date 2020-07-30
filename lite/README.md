# TensorFlow Lite sample applications

<!-- Note: These samples are being staged internally before being migrated to
     the new TF examples repo. See also b/119060183. -->

The following samples demonstrate the use of TensorFlow Lite in mobile applications. Each sample is written for both Android and iOS.

## Image classification

This app performs image classification on a live camera feed and displays the
inference output in realtime on the screen.

<!-- TODO(b/124116863): Add app screenshot and model details. -->

### Samples

[Android image classification](examples/image_classification/android/README.md)

[iOS image classification](examples/image_classification/ios/README.md)

[Raspberry Pi image classification](examples/image_classification/raspberry_pi/README.md)

## Object detection

这个应用程序在一个实时摄像头上执行对象检测，并在屏幕上实时显示结果。该应用程序显示多个对象的信心分数、类和检测到的边界框。只有当置信度分数大于定义的阈值时，才显示检测到的对象。

<!-- TODO(b/124116863): 添加应用程序截图和模型细节 -->

### Samples

[Android object detection](examples/object_detection/android/README.md)

[iOS object detection](examples/object_detection/ios/README.md)

[Raspberry Pi object detection](examples/object_detection/raspberry_pi/README.md)


## Speech command recognition

This application recognizes a set of voice commands using the device's microphone input. When a command is spoken, the corresponding class in the app is highlighted.

<!-- TODO(b/124116863): Add app screenshot and model details. -->

### Samples

[Android speech commands](examples/speech_commands/android/README.md)

[iOS speech commands](examples/speech_commands/ios/README.md)


## Gesture classification

This app uses a model to classify and recognize different gestures. A model is trained on webcam data captured using a web interface. The model is then converted to a TensorFlow Lite model and used to classify gestures in a mobile application.

![Gesture components](https://tensorflow.org/images/lite/screenshots/gesture_components.png)

### Web app

First, we use TensorFlow.js embedded in a web interface to collect the data required to train the model. We then use TensorFlow.js to train the model.

[Web gesture classification](examples/gesture_classification/web/README.md)

<!-- TODO(b/124116863): Add app screenshot and model details. -->

### Conversion script

The model downloaded from the web interface is converted to a TensorFlow Lite model.

[Conversion script (available as a Colab notebook)](examples/gesture_classification/ml/README.md).

### Mobile apps

Once we have the TensorFlow Lite model, the implementation is very similar to the [Image classification](#image-classification) sample.

<!-- TODO(b/124116863): Add app screenshot. -->

#### Samples

[Android gesture classification](examples/gesture_classification/android/README.md)

[iOS gesture classification](examples/gesture_classification/ios/README.md)

## Model personalization

This app performs model personalization on a live camera feed and displays the
results in realtime on the screen. The app displays the confidence scores,
classes and detected bounding boxes for multiple objects that were trained in
realtime.

<!-- TODO(b/124116863): Add app screenshot and model details. -->

### Samples

[Android Model Personalization](examples/model_personalization/README.md)


