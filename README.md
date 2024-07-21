# UNET

- The model Architecture is copied and converted into Pytorch from the this [medium article](https://medium.com/geekculture/u-net-implementation-from-scratch-using-tensorflow-b4342266e406)
- The data download, pre-processing and training and testing function are directly copied from this [Kaggle notebook](https://www.kaggle.com/code/dhruv4930/oxford-iiit-pets-segmentation-using-pytorch)
- Dice loss implemented on top of these for experiment 2 and 4


## Experiment1: MP+Tr+CE - [notebook](https://github.com/sayanbanerjee32/UNET/blob/main/UNET_MP_TR_CE.ipynb)

Important features of model architecture:
1.  Method of reducing feature size in encoder: MaxPooling
2.  Method of increasing feature size in decoder: Transpose Convolution
3.  Loss function: Cross Entropy

### Performance
- Pixel accuracy: 90%
- IoU Metric: 75%

### Output
![image](https://github.com/user-attachments/assets/084ca21e-316a-4a5d-aa64-40550fcab88b)

## Experiment2: MP+Tr+Dice Loss - [notebook](https://github.com/sayanbanerjee32/UNET/blob/main/UNET_MP_TR_DiceLoss.ipynb)
Important features of model architecture:
1.  Method of reducing feature size in encoder: MaxPooling
2.  Method of increasing feature size in decoder: Transpose Convolution
3.  Loss function: Dice loss

### Performance
- Pixel accuracy: 89%
- IoU Metric: 72%

### Output
![image](https://github.com/user-attachments/assets/93a956ca-9242-412b-8e39-b4902714ec5e)


## Experiment3: StrConv+Tr+CE - [notebook](https://github.com/sayanbanerjee32/UNET/blob/main/UNET_StrConv_TR_CE.ipynb)
Important features of model architecture:
1.  Method of reducing feature size in encoder: Strided Convolution
2.  Method of increasing feature size in decoder: Transpose Convolution
3.  Loss function: Cross Entropy

### Performance
- Pixel accuracy: 90%
- IoU Metric: 75%

### Output
![image](https://github.com/user-attachments/assets/3312f7b5-56a1-43dc-965e-828beb3ab247)


## Experiment4: StrConv+Ups+Dice Loss - [notebook](https://github.com/sayanbanerjee32/UNET/blob/main/UNET_StrConv_UpSamp_DiceLoss.ipynb)
Important features of model architecture:
1.  Method of reducing feature size in encoder: Strided Convolution
2.  Method of increasing feature size in decoder: Upsampling
3.  Loss function: Dice loss

### Performance
- Pixel accuracy: 90%
- IoU Metric: 76%

### Output
![image](https://github.com/user-attachments/assets/8538dace-86ae-4328-ad5f-3c6a87197643)
