<img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/Logo.png" align="right">

# WasteKart2

WasteKart is the App which help End Customers to scan their waste and get relevant information instantly along with estimated price range through inbuild object detection manich learning alrogrithm.

WasteKart leveraging the power of [TensorFlow 2.x Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection) to detect specifc class of waste and suggest price range by calling External API deployed on SAP BTP platform.

WasteKart is using Transfer Learning technique to train custom object detection model by using pre-trained model [efficientdet_lite2](https://tfhub.dev/tensorflow/lite-model/efficientdet/lite2/detection/metadata/1) on custom dataset - Laptop & Mobile phone.

To understand better, here is the good [tutorial](https://codelabs.developers.google.com/tflite-object-detection-android) available.

The dataset used for Laptop and Mobile phone is [Open Images](https://storage.googleapis.com/openimages/web/index.html)

Please follow [Google Colab](https://colab.research.google.com/drive/1LhsI0LyJszN_0WjpHJIAKoV87vegQWkH?usp=sharing) to see how training done on custom dataset and how tensorflow lite model is extracted to be used.

## Installation Setup

Application can run either on device or emulator.

### Prerequisites
* If you don't have already, install [Android Studio](https://developer.android.com/studio/index.html), following the instructions on the website.
* You need an Android device and Android development environment with minimum API 21.
* Android Studio 3.2 or later.

### Building
* Open Android Studio, and from the Welcome screen, select Open an existing Android Studio project.
* From the Open File or Project window that appears, select WasteKart directory from wherever you cloned. Click OK.
* If it asks you to do a Gradle Sync, click OK.
* You may also need to install various platforms and tools, if you get errors like "Failed to find target with hash string 'android-21'" and similar. Click the Run button (the green arrow) or select Run > Run 'android' from the top menu. You may need to rebuild the project using Build > Rebuild Project.
* If it asks you to use Instant Run, click Proceed Without Instant Run.
* Also, you need to have an Android device plugged in with developer options enabled at this point. See [here](https://developer.android.com/studio/run/device) for more details on setting up developer devices.

## Price Recommendation API

### Application Route
https://price-recomm-srv-mediating-porcupine-gj.cfapps.us10.hana.ondemand.com/

### API used by APP
https://price-recomm-srv-mediating-porcupine-gj.cfapps.us10.hana.ondemand.com/price-recomm/Products?$expand=category,price

## Demo

<img src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/Demo_Video.gif" width="250" height="400"/>


## Gallery

<p align="left" width="100%">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic1.jpeg">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic2.jpeg">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic3.jpeg">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic4.jpeg">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic5.jpeg">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic6.jpeg">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic7.jpeg">
    <img width="15%" src="https://github.com/KapilSAP/WasteKart2/blob/main/gallery/pic8.jpeg">
</p>

## Roadmap
* Display Recycle Guide based on detected object
* [Geofire](https://github.com/firebase/geofire-android) Integration to find nearest ragman
