# WasteKart2

WasteKart is the App which help End Customers to scan their waste and get relevant information instantly along with estimated price range through inbuild object detection manich learning alrogrithm.

WasteKart leveraging the power of [TensorFlow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection) to detect specifc class of waste and suggest price range by calling External API deployed on SAP BTP platform.

WasteKart is using Transfer Learning technique to train custom object detection model by using pre-trained model [efficientdet_lite2](https://tfhub.dev/tensorflow/lite-model/efficientdet/lite2/detection/metadata/1) on custom dataset - Laptop & Mobile phone.

To understand better, here is the good [tutorial](https://codelabs.developers.google.com/tflite-object-detection-android) available.


## Installation Setup
