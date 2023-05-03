# YogaNet

This is a model for classification of yoga poses using human activity recognition (HAR). The goal is to train a robust model that can accurately classify the yoga pose being performed in a video feed in real time. Libraries used are [MediaPipe](https://developers.google.com/mediapipe) and [TensorFlow](https://www.tensorflow.org/). I am currently still working on this project and further testing is required to achieve the results promised in the study.

## Details

The model is created using [TensorFlow](https://www.tensorflow.org/). The video data used to train the model is first fed to [MediaPipe](https://developers.google.com/mediapipe) to extract the key points of the person performing the yoga pose. These key points are then fed to the model using a custom time-series data loader that is then used to train it. The metrics used for evaluation are loss, accuracy and confusion matrix. The train-validation-test split is 64:16:20 (as per the cited study).

## References

Swain, D.; Satapathy, S.; Acharya, B.; Shukla, M.; Gerogiannis, V.C.; Kanavos, A.; Giakovis, D. Deep Learning Models for Yoga Pose Monitoring. *Algorithms* **2022**, *15*, 403. https://doi.org/10.3390/a15110403
