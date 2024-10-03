# Brain Tumor Segmentation

This project focuses on brain tumor segmentation using deep learning models. Two architectures, **U-Net** and **ResU-Net**, have been implemented to perform segmentation on MRI images to distinguish between tumor and non-tumor regions.

## Project Overview
Brain tumor segmentation is a critical task in medical image analysis, particularly in MRI scans where tumors need to be distinguished from healthy tissues. Manual segmentation is time-consuming and prone to errors, making automated deep learning-based approaches highly beneficial.

This project implements two convolutional neural network models, U-Net and ResU-Net, both widely used for medical image segmentation tasks. The models are trained to segment tumor regions in MRI brain images.

## Models
### 1. U-Net
U-Net is a fully convolutional neural network designed for biomedical image segmentation. It uses an encoder-decoder structure to learn high-level representations and recover spatial resolution through skip connections. It is implemented in the Unet_Brain_Tumor_Segmentation.ipynb notebook.

### 2. ResU-Net
ResU-Net extends U-Net by incorporating residual connections, which help in training deeper networks by alleviating the vanishing gradient problem. It is implemented in the Res_UNet_Brain_Tumor_Segmentation.ipynb notebook.

Both notebooks include sections for loading data, preprocessing, model training, and evaluation.

## Dataset
The dataset used for training and testing the models is the BRATS 2020 Dataset [1]. The BRATS dataset focuses on the automatic segmentation of brain tumors from multi-modal MRI scans. Its main objective is to enable accurate detection and delineation of tumor sub-regions, which is critical for diagnosis, treatment planning, and follow-up assessment. The dataset consists of over 369 cases with MRI volumes, each accompanied by manually labeled ground truth segmentations. The segmentation masks correspond to the above sub-regions and are used as training labels for model development.

## Evaluation Metric
The models are trained and evaluated using the Dice coefficient. It measures the overlap between the predicted segmentation and the ground truth. It ranges from 0 to 1, where a Dice score of 1 indicates perfect overlap and 0 indicates no overlap. Specific results and model performance can be found in the respective Jupyter notebooks.

## References
[1] https://www.med.upenn.edu/cbica/brats2020/data.html

