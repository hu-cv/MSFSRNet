# MSFSRNet
Hi! You are welcome to visit here! This repository will be used to release the code of a novel image restoration model called the Residual Network with Multi-skip Feature Sharing (abbreviated as MSFSRNet), which has been proposed in our paper entitled "MSFSRNet: Residual Network with Multi-skip Feature Sharing for Image Restoration" submitted to the International journal of XXX. **NOTE that once our manuscript is accepted by the journal, we will release the code immediately**. 
## Abstract
 <p>这是需要对齐的段落。 </p> text-align: justify; text-justify: inter-word; </style>
 <p> &emsp;&emsp;Residual dense network-based models have been widely and successfully used in the field of image restoration in recent years because of their enhanced feature propagation and anti-overfitting capabilities. However, existing residual dense network-based models have the following defects: 1) The convolution blocks in the model usually use dense connections, so that local features are captured repeatedly, which adds too many redundant features. 2) Each layer in the convolution block contains only one convolution layer, which reduces the representation ability of the convolution block, resulting in poor results in extracting local features by the convolution block. 3) The convolution blocks form a feature flow through simple connections, making it difficult to effectively fuse global features, which results in the lack of detail information in the reconstructed image. To overcome the shortcomings of residual dense network-based models, this paper addresses the problem of image restoration by proposing a novel image restoration model called the Residual Network with Multi-skip Feature Sharing (abbreviated as MSFSRNet). In MSFSRNet, the dense connections in the residual dense network are replaced with multi-skip connections to form a multi-skip feature sharing residual block (MSFSRB), which reduces the number of redundant features. Each layer in MSFSRB contains two convolutional layers, called multi-skip feature sharing convolutional layers (MSFSConv), which improves the extraction of local features in MSFSRB. In addition, we insert a feature enhancement layer after each MSFSRB to better integrate global features. Extensive experiments on 11 synthetic datasets and real-world datasets show that our MSFSRNet model outperforms the state-of-the-art models in two image restoration tasks including image super-resolution and image denoising. </p> text-align: justify; text-justify: inter-word; </style>
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

References: <br>
[1] Julien Mairal, Francis R. Bach, Jean Ponce, Guillermo Sapiro, Andrew Zisserman: Non-local sparse models for image restoration. IEEE 12th International Conference on Computer Vision, ICCV 2009: 2272-2279. https://doi.org/10.1109/ICCV.2009.5459452 <br>
[2] Stefan Roth, Michael J. Black:Fields of Experts: A Framework for Learning Image Priors.2005 IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR 2005), 20-26 June 2005, San Diego, CA, USA.: 860-867. https://doi.org/10.1109/CVPR.2005.160 <br>
[3] Franzen R (1999) Kodak lossless true color image suite vol 4, https://r0k.us/graphics/kodak. <br>
[4] Lei Zhang, Xiaolin Wu, Antoni Buades, Xin Li: Color demosaicking by local directional interpolation and nonlocal adaptive thresholding. J. Electronic Imaging 20(2): 023016 (2011). https://doi.org/10.1117/1.3600632 <br>
[5] Marco Bevilacqua, Aline Roumy, Christine Guillemot, Marie-Line Alberi-Morel:Low-Complexity Single-Image Super-Resolution based on Nonnegative Neighbor Embedding. BMVC 2012: 1-10. https://doi.org/10.5244/C.26.135 <br>
[6] Roman Zeyde, Michael Elad, Matan Protter:On Single Image Scale-Up Using Sparse-Representations. Curves and Surfaces 2010: 711-730. https://doi.org/10.1007/978-3-642-27413-8_47 <br>
[7] David R. Martin, Charless C. Fowlkes, Doron Tal, Jitendra Malik: A Database of Human Segmented Natural Images and its Application to Evaluating Segmentation Algorithms and Measuring Ecological Statistics. Proceedings of the Eighth International Conference On Computer Vision (ICCV-01), Vancouver, British Columbia, Canada, July 7-14, 2001: 416-425. https://doi.org/10.1109/ICCV.2001.937655. <br>
[8] Jia-Bin Huang, Abhishek Singh, Narendra Ahuja:Single image super-resolution from transformed self-exemplars.IEEE Conference on Computer Vision and Pattern Recognition, CVPR 2015, Boston, MA, USA, June 7-12, 2015.:5197-5206. https://doi.org/10.1109/CVPR.2015.7299156 <br>
[9] Yusuke Matsui, Kota Ito, Yuji Aramaki, Azuma Fujimoto, Toru Ogawa, Toshihiko Yamasaki, Kiyoharu Aizawa:Sketch-based manga retrieval using manga109 dataset. Multim. Tools Appl. 76(20): 21811-21838 (2017). https://doi.org/10.1007/s11042-016-4020-z. <br>

# Experimental Results
