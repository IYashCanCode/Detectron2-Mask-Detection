# Detectron2-Mask-Detection
Problem Statement : Creating a Detectron2 custome object detection model to detect Mask.

Dataset link : https://www.kaggle.com/datasets/aditya276/face-mask-dataset-yolo-format


# Mask detection on detectron2 colab file

The detectron model used for creating this model is 'faster_rcnn_R_50_C4', a prebuild model present in detectron2 model_zoo module.

The input data is first annotated using LabelMe annotation tool, there are 2 classes made on the training and testing images named 'Mask' and 'No Mask'. After annotating the images the json format is converted into desired COCO format required by detectron2.

There 1035 training dataset instances in which 885 instances are of 'Mask' and 150 are of 'No Mask' and for testing there are 60 total instances out of which 32 are of 'Mask' and 28 of 'No Mask'.

The model is trained on CUDA processor on 128 images per batch for 500 iterations

# Results of model
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/47146b67-8da2-40de-9467-c42d36aa115d)

