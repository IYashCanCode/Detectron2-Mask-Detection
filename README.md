# Detectron2-Mask-Segmentation
Problem Statement : Creating a Detectron2 custome object segmentation model to detect Mask.

Dataset link : https://www.kaggle.com/datasets/aditya276/face-mask-dataset-yolo-format


# Mask segmentation on detectron2 colab file

The detectron model used for creating this model is 'mask_rcnn_R_101_FPN_3x', a prebuild model present in detectron2 model_zoo module.

The input data is first annotated using LabelMe annotation tool, there are 2 classes made on the training and testing images named 'Mask' and 'No Mask'. After annotating the images the json format is converted into desired COCO format required by detectron2.

There 1035 training dataset instances in which 885 instances are of 'Mask' and 150 are of 'No Mask' and for testing there are 60 total instances out of which 32 are of 'Mask' and 28 of 'No Mask'.

The model is trained on CUDA processor on 128 images per batch for 500 iterations

# Results of model
The images below are the models prediction to detect the two classes 'Mask' and 'No Mask'

# Predicted annoatations 
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/2bebda70-721e-40e6-a633-ba22e0b854cf)

 
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/638231cf-1dd6-473e-b02d-99215df14254)



# Model Evaluation 

On training images the model is able to get around 71% AP (Average Precision)
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/330a0c0a-0b5d-4ed9-bc22-8373fa7d4a83)


On testing images the model is able to get around 70% AP (Average Precision)
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/5ba99d51-961a-4348-aead-522512d07242)



#
# Flask API
#
For this model a flask API is created to interact to the model over internet.

# User Interface of Flask API
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/7d8107fd-a865-42cd-9986-f780946a76f0)


# Results on Flask API
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/396114ca-bc94-4faf-be15-b782d608d6c4)

![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/251696f7-bd81-429f-b74a-0ecaa994b767)

![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/5047cf1f-fe85-4495-97ca-19ab88308703)

![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/c2221dd2-2607-4313-bb79-09fe2c7d7150)



#
# Streamlit API
#
For this model a Streamlit API is created to interact to the model over internet.

# User Interface of Streamlit API
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/f50af214-df7e-42b4-b244-40dc162f4de2)


Once you upload an image it will caption it with the text uploaded images and provide a predict button to predict the classes in the images

# Results on Streamlit API
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/ee43e353-963c-44a9-a519-6ad8c9b46c9e)
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/2a4dd111-32e5-4274-b315-c62bfeef78a7)

# THANK YOU 







