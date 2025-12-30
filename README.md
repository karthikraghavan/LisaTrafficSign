# LisaTrafficSign
This project aims to perform automatic detection and recognition of traffic road signs. The project analyzes images and labels of road signs like Stop signs, pedestrian crossings, or speed limits and aims to recognize American types of road signs.

#Dataset Analysis

The LISA Road sign dataset published by Roboflow. is used for traffic detection. Roboflow publishes datasets in various formats, including YOLO, XML, JSON, and TFRecord.

Train:        9926
Validation:	  993
Test:        	662
Img size:    	416x416
Number of 
classes:	    48

### Class distribution plot

<img width="468" alt="image" src="https://github.com/user-attachments/assets/3971fc65-17f3-4bcf-a1d5-f38351f24891">

### Image augmentation

Open CV uses the following preprocessing techniques to augment images
•	Histogram Equalization
•	CLAHE 
•	Image Sharpening 
•	Denoising 

<img width="468" alt="image" src="https://github.com/user-attachments/assets/ad05f575-a2ab-460a-8616-75fc04c2253c">

Train dataset:                                        	9926
Train dataset after image preprocessing & augmentation:	49630

# Model Training & Evaluation

1. Yolo version: Yolov10n
2. Environment: MAC with M3 max chip
3. Model Training
    Iteration 1 – Raw dataset
    Iteration 2 – Pre-processed images

# Model Inference


Precision
Recall
mAP50
mAP50-95
Raw dataset
66.5
62.7
63.8
50
Pre-processed dataset
83.1
75.5
87.8
70.7
<img width="631" alt="image" src="https://github.com/user-attachments/assets/ca03765f-3c46-4ba8-9b35-416422089b37">


### Confusion Matrix

<img width="661" alt="image" src="https://github.com/user-attachments/assets/4416e2c7-259d-475b-85eb-53252bb45675">

### Loss and Evaluation metrics

<img width="591" alt="image" src="https://github.com/user-attachments/assets/5f5324f9-68e3-424b-bd83-6e730c00094d">


# Conclusion

1. Traffic sign detection ended with a mean average precision score of 87.8% with 50% IOU threshold.
2. Use GAN for image augmentation
3. Train on additional diverse datasets beyond LISA 
4. Train on additional architectures like RETINET, Faster-CNN
5. Implement Pedestrian/Lane detection 
6. Optimize hyperparameters
7. Employ methods for more efficient training and memory optimization

















