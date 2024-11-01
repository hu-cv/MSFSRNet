# MSFSRNet
Hi! You are welcome to visit here! This repository will be used to release the code of a novel image restoration model called the Residual Network with Multi-skip Feature Sharing (abbreviated as MSFSRNet), which has been proposed in our paper entitled "MSFSRNet: Residual Network with Multi-skip Feature Sharing for Image Restoration" submitted to the International journal of XXX. **NOTE that once our manuscript is accepted by the journal, we will release the code immediately**. 
Residual dense network-based models have been widely and successfully used in the field of image restoration in recent years because of their enhanced feature propagation and anti-overfitting capabilities. However, existing residual dense network-based models have the following defects: 1) The convolution blocks in the model usually use dense connections, so that local features are captured repeatedly, which adds too many redundant features. 2) Each layer in the convolution block contains only one convolution layer, which reduces the representation ability of the convolution block, resulting in poor results in extracting local features by the convolution block. 3) The convolution blocks form a feature flow through simple connections, making it difficult to effectively fuse global features, which results in the lack of detail information in the reconstructed image. To overcome the shortcomings of residual dense network-based models, this paper addresses the problem of image restoration by proposing a novel image restoration model called the Residual Network with Multi-skip Feature Sharing (abbreviated as MSFSRNet). In MSFSRNet, the dense connections in the residual dense network are replaced with multi-skip connections to form a multi-skip feature sharing residual block (MSFSRB), which reduces the number of redundant features. Each layer in MSFSRB contains two convolutional layers, called multi-skip feature sharing convolutional layers (MSFSConv), which improves the extraction of local features in MSFSRB. In addition, we insert a feature enhancement layer after each MSFSRB to better integrate global features. Extensive experiments on 11 synthetic datasets and real-world datasets show that our MSFSRNet model outperforms the state-of-the-art models in two image restoration tasks including image super-resolution and image denoising.
# Experimental Datasets
## Image Denoising
###  Gray-Scale Image Denoising
* **BSD68** 
* **Set12**
###  Synthetic Color Image Denoising
* **CBSD68**
* **McMaster**
* **Kodak24**
###  Real-World Color Image Denoising
* **SIDD**
* **DND**
## Image super-resolution
* **Set5**
* **Set14**
* **BSD100**
* **Urban100**
* **Manage109**
# Experimental Results
