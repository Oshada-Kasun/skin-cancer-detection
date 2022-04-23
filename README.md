# Skin cancer detection using Deep Neural Networks

It is important to detect skin cancer and treat it at an initial stage to improve the overall survival rate in humans. This would also lead to a reduction in turnaround time in medical diagnosis by the oncologist, leading to more patient inflow per day in the hospital.
Project aims to tackle this problem by implementing deep learning frameworks to detect skin cancer diseases with high confidence.

## Model development
* EfficientNet B3, B4, B5 and B6, InceptionV3, and VGG19 pre-trained networks data augmentation on malignant images, fine-tuning, hyper-parameter tuning, overall test performance is reached 0.81 F1-score for VGG-19 model.

* Included explainable AI using GradCam to generate heatmaps to improve confidence and reliability of results.

* The skin images are randomly selected without regard to the age, sex and the type of diagnosis to avoid representation bias in the data.

## Web app Development and Deployment

* The heatmaps are generated using Grad-CAM (Gradient-weighted Class Activation Mapping) to incorporate Explainable AI. After that the trained model has been saved into TFLite  and H5 file formats for the deployment purpose. 

* Developed as a Web App, using Fast API, for producing predictions (whether it is malignant or benign) along with the associated confidence value of that prediction and the heatmap.

* Finally, the Web App is containerized using Docker and deployed via AWS using the EC2 instance with configuring all necessary components . 
