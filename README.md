# Exploration-of-novel-deep-learning-methods-for-Edge-Detection

This is a machine learning project focusing on computer vision. The goal is this project is to explore deep learning methods for detecting edges in images and compare their performance. Edge Detection aims to find regions in an image where there is a sharp change in intensity or color.

There are two parts in this project: my teammate did Traditional Method Inspired Deep Neural Network for Edge Detection and I did Enhanced Richer Convolutional Features (ERCF) For Edge Detection, which takes VGG19 as a backbone and trains the model with CNN. My model is inspired by Yun Liu, the author of RCF model, as well as several Github contributors (links per below):
https://github.com/balajiselvaraj1601/RCF_Pytorch_Updated
https://github.com/Walstruzz/edge_eval_python

The dataset utilized in this project is BSDS500, which is a popular dataset for edge detection.

Model design:
![image](https://user-images.githubusercontent.com/75347096/132914105-3e972c01-fc0b-4d3a-b675-2fb941b9688f.png)

Model results:
![image](https://user-images.githubusercontent.com/75347096/132914163-a9c62548-e8a7-4128-a399-04297f9ff947.png)
![image](https://user-images.githubusercontent.com/75347096/132914170-c075d1e2-3364-4d0d-961d-b8b597ed5e55.png)

![image](https://user-images.githubusercontent.com/75347096/132914222-7cfa60c5-45e7-4816-b786-2c34b55c1fbe.png)
![image](https://user-images.githubusercontent.com/75347096/132914236-24896bfb-49ce-4404-a246-ad243c748ae5.png)

For model evaluation, there are two industry standard metrics to measure model performance. The first one is referred as optimal dataset scale (ODS) which employs a fixed threshold for all images in a dataset. The second is called optimal image scale (OIS) which selects an optimal threshold for each image. For the two metrics, the higher the better.

	            ODS	      OIS
RCF	          0.757982	0.775395
enhanced RCF	0.761043	0.776080

Note the model evaluation part can only be executed in Linux. The CUDA is also enabled in the notebook.
