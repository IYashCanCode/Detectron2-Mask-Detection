# Detectron2-Mask-Detection
Problem Statement : Creating a Detectron2 custome object detection model to detect Mask.

Dataset link : https://www.kaggle.com/datasets/aditya276/face-mask-dataset-yolo-format


# Mask detection on detectron2 colab file

The detectron model used for creating this model is 'faster_rcnn_R_50_C4', a prebuild model present in detectron2 model_zoo module.

The input data is first annotated using LabelMe annotation tool, there are 2 classes made on the training and testing images named 'Mask' and 'No Mask'. After annotating the images the json format is converted into desired COCO format required by detectron2.

There 1035 training dataset instances in which 885 instances are of 'Mask' and 150 are of 'No Mask' and for testing there are 60 total instances out of which 32 are of 'Mask' and 28 of 'No Mask'.

The model is trained on CUDA processor on 128 images per batch for 500 iterations

# Results of model
The images below are the models prediction to detect the two classes 'Mask' and 'No Mask'

# Original image
![160](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/7772e6f2-f0cc-4a18-9fac-e88ee2109bfe)

# Predicted annoatations 
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/2bebda70-721e-40e6-a633-ba22e0b854cf)


# Original image
![1_R_kFK9pNLfKAuopY_lAaPQ](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/37ec9456-2139-4a07-b019-456177910dcb)

# Predicted annoatations 
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
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/ecd782ac-8fc3-42e0-a647-7b276b666f84)


# Results on Flask API
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/7331cfb9-1e71-42db-87de-ea62647cf1a6)

![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/bf41e1c4-2c9e-46c8-98dc-6691aec99d61)


![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/dd6aabb6-693a-4a84-97ee-6b5cf11be42b)

![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/1567d777-983f-4502-9f5d-c78e2baa38e8)


#
# Streamlit API
#
For this model a Streamlit API is created to interact to the model over internet.

# User Interface of Flask API
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/83b3bacb-b78a-42ce-833f-9ac634e0759f)

Once you upload an image it will caption it with the text uploaded images and provide a predict button to predict the classes in the images

# Results on Streamlit API
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/b6b1a4fa-ef62-405e-b056-cbfe67feba41)
![image](https://github.com/IYashCanCode/Detectron2-Mask-Detection/assets/91466909/0450a4dc-398b-479a-b84c-2f09a5012dc2)

# THANK YOU 







