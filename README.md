# CSCE-5210_AI_Class-Project
## Introduction
In this paper, we utilizes the CNNs approach for facial emotion recognition. We trained and tested our model on the FER2013 dataset which consists of 48x48 pixel grayscale images of faces. The images are format into a .csv file with 2 columns. The first column is consented of the labels and it has the different 'emotions' (0) angry, (1) disgusted, (2) fearful, (3) happy, (4) sad, (5) surprised, (6) neutral. The second column is the 'data' which are the different pixels in the images. The total count was 30000 images in our dataset.
![image](https://user-images.githubusercontent.com/78702377/116769307-b185f400-aa00-11eb-972a-1a88476c7476.png)


## Method
The hardware environment of this experiment is asfollows: Window10 operating system, Intel i7-7700KCPU, NVIDIA GeForce GTX 1080 Ti GPU hardwareenvironment.  The software environment is Python3.6.8 with PyTorch, and CUDA 11.1 is used to builda convolution neural network. Our network has three convolution layers and onefully connected layer.  Shown in Figure 3.  In thefirst convolution layer, we had 64 filters with kernelsize is 3x3. The second convolution is different fromfirst layer. In this layer, we have 128 3x3 filters. Thethird convolution layers has 256 3x3 filters.  Theseconvolution layers also along with batch normaliza-tion, max-pooling layer and dropout. Pooling setupis 2x2 with a stride of 1 to reduce the size of the re-ceptive field and avoid overfitting. In dropout layer,a fraction of 0.2 is used.
![CNN architecture](https://user-images.githubusercontent.com/78702377/116769334-ec882780-aa00-11eb-82a5-32f1e8573b7e.png)
