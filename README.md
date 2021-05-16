# RIP_object_detection
Simple Android Project using OpenCV, Mobilnet net based on COCO dataset

Tutorial and simple Code:
https://github.com/tintintin/android-opencv-example
https://zen.yandex.ru/media/id/5cafa05b0a588d00b0a57bad/pishem-prosteishee-prilojenie-pod-android-dlia-raspoznavaniia-obektov-s-kamery-5e624bfa824a2d437a810a71

model of net from
https://github.com/chuanqi305/MobileNet-SSD

important notes:

1)Make sure that compileSdkVersion & targetSdk Version are the smae in all gradle files
2) import module of OpenCV-sdk/java

3)add arm64-v8a/libc++_.shared.so,...,...,..., from(somehow?) NDK and native libs fromOpenSdk to jnilibs

4)make folders jniLibs and assets in project/app/src/main

5)insert model of net and wages into assets

Additional info:
!!!OpenCV package manager is deprecated!!!
!!!u should link OpenCV librarry as ststic (it was not recommennded in previous years ~2019?, now (2021 statick linking is only way, package manager disappeared, u cannot install it)
fast import of open CV library:
https://github.com/seesaa/opencv-android

old tutorial, doesnt work but contains simple code structure
https://docs.opencv.org/3.4/d0/d6c/tutorial_dnn_android.html

using camera in openCV, android, simple code
https://www.youtube.com/watch?v=A4-wkW54scM
https://www.youtube.com/watch?v=ZTQBbnWkFV4



%%%% preparing model %%%%%
collect data-> label data
labeling
https://github.com/tzutalin/labelImg

transform data and labels
https://github.com/Tony607/object_detection_demo
https://www.dlology.com/blog/how-to-train-an-object-detection-model-easy-for-free/
https://www.youtube.com/watch?v=kq2Gjv_pPe8 xml->csv- preparing tfrecords

my simple script is uploaded on this repo, u need to have the same file structures as me(hardcoded paths):
images/train/your_images_with_labels_1
images/test/your_images_with_labels_2
data

====Next Level=======


