# Exploration-of-novel-deep-learning-methods-for-Edge-Detection

This is a machine learning project focusing on computer vision. The goal is this project is to explore deep learning methods for detecting edges in images and compare their performance. Edge Detection aims to find regions in an image where there is a sharp change in intensity or color.

There are two parts in this project: my teammate did Traditional Method Inspired Deep Neural Network for Edge Detection and I did Enhanced Richer Convolutional Features (ERCF) For Edge Detection, which takes VGG19 as a backbone and trains the model with CNN. My model is inspired by Yun Liu, the author of RCF model, as well as several Github contributors (links per below):
https://github.com/balajiselvaraj1601/RCF_Pytorch_Updated
https://github.com/Walstruzz/edge_eval_python

The dataset utilized in this project is BSDS500, which is a popular dataset for edge detection.

Model design:

![image](https://user-images.githubusercontent.com/75347096/132914105-3e972c01-fc0b-4d3a-b675-2fb941b9688f.png)

Model results:

![image](https://user-images.githubusercontent.com/75347096/132917991-110a6c88-2175-4faa-b232-eaadc526d3c2.png)
![image](https://user-images.githubusercontent.com/75347096/132918005-e161d4fc-5163-480d-9dbf-bd192e56f73f.png)

![image](https://user-images.githubusercontent.com/75347096/132918020-a43dbb41-e4ce-4d5b-b4fc-a65e440a2c8d.png)
![image](https://user-images.githubusercontent.com/75347096/132918028-24ad84c3-3afb-408e-af9b-b26e64e45576.png)

For model evaluation, there are two industry standard metrics to measure model performance. The first one is referred as optimal dataset scale (ODS) which employs a fixed threshold for all images in a dataset. The second is called optimal image scale (OIS) which selects an optimal threshold for each image. For the two metrics, the higher the better.

ODS	        OIS
		  
RCF	        0.757982	0.775395

enhanced RCF	0.761043	0.776080

Note the model evaluation part can only be executed in Linux. The CUDA is also enabled in the notebook.
