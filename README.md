# CNN Image Segmenation
![image-segmentation-background](https://github.com/user-attachments/assets/1966be79-08ae-433e-a61f-a5061a4460fa)

## Introduction
This project implement some CNN based image segmentation models.
This project showcases my work in image segmentation using deep Convolutional Neural Networks (CNNs). It features various CNN models designed for segmentation tasks, most of which are based on the encoder-decoder architecture. The key differences among these models lie in the choice of encoder networks for feature extraction and the integration of attention mechanisms to enhance accuracy and focus on critical regions in feature maps.
The attention modules included in this project primarily predate before 2020, providing insights into their effectiveness. Actually, this project reviews cost-effective approaches for implementing attention mechanisms in image segmentation.

---
## Different Models
- #### UNet-ResNet18
    - Using ResNet18 as a backbone for the UNet network
    - <a href= 'https://arxiv.org/abs/1512.03385'> ResNet Article </a>
     <br>
- #### UNet-ResNet18-AG
    - Using ResNet18 as a backbone and Attention Gate module as Attention module for the UNet network
    - <a  href="https://arxiv.org/abs/1804.03999v3"> AG Article </a>
    <br>
     <img  src= "https://production-media.paperswithcode.com/methods/25b72303-3ebf-4db0-a6bd-f141e5c8c114.jpg" />

     <img src= 'https://github.com/ozan-oktay/Attention-Gated-Networks/blob/master/figures/figure1.png?raw=true' />
    <br>
- #### UNet-ResNet18-scSE
    - Using ResNet18 as a backbone and spatial-channel Squeeze and Excitation module as Attention module for the UNet network
    - <a href="https://arxiv.org/abs/1808.08127v1"> scSE 
    Article </a>
    <img src = 'https://production-media.paperswithcode.com/methods/scSE_Block_YcKqn9P.png' />
    <br>
- #### UNet-ResNeXt18
    - Using ResNeXt-18 as a backbone for the UNet network
    - <a href='https://arxiv.org/abs/1611.05431'> ResNeXT Article </a>
    <br>
    <img src='https://production-media.paperswithcode.com/methods/Screen_Shot_2020-06-06_at_4.32.52_PM.png' />

- #### UNet-ConvNeXt
    - Using ConvNeXT large as a backbone for the UNet network
    - <a href ='https://arxiv.org/abs/2201.03545'> ConvNeXt Article </a>
    <br>
    <img src='https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/convnext_architecture.jpg' a>
    <br>

- #### MANet-ResNeXt
    - Using ResNeXT as backbone for the MANet network
    - <a  href = 'https://arxiv.org/abs/2009.02130'> MANet Article </a>
    <br>
    
    <br>

- #### MANet-ResNet
    - Using ResNet as backbone for the MANet network

--
## Installation
 - These models are written in the **Pytorch** library
- torch `2.6`
- torchvision `0.21.0`
- tqdm `4.6.1`
- python `3.10+`
- torchmetrics 
- early-stopping-pytorch

 ##### Install torch and torchvision from Pytorch Locally
 ```diff
pip3 install torch==2.6 torchvision==0.21.
```
##### Install early-stopping-pytorch and torchmetrics from PyPI
``` diff
pip install early-stopping-pytorch
pip install torchmetrics
```
## References


I have used  functions from other great open-source projects. Espeicially thank the authors of:
- https://github.com/ozan-oktay/Attention-Gated-Networks
- https://github.com/facebookresearch/ConvNeXt
- https://github.com/kevinkwshin/MANet
- https://github.com/ai-med/squeeze_and_excitation
