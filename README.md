# MSFSRNet
Hi! You are welcome to visit here! This repository will be used to release the code of a novel image restoration model called the  Multi-skip feature sharing residual network&ensp;(abbreviated as MSFSRNet), which has been proposed in our paper entitled "MSFSRNet:  Multi-skip feature sharing residual network for image restoration" submitted to the International journal of **Machine Vision and Applications**. **NOTE that once our manuscript is accepted by the journal, we will release the code immediately**. 
## Abstract

 <p> Residual dense network-based models have been widely used in the field of image restoration in recent years because of their enhanced feature propagation and anti-overfitting capabilities. However, existing residual dense network-based models have the following shortcomings: 1) The dense connections between convolutional blocks in these models lead to feature redundancy by repeatedly capturing local features. 2) Each convolution block contains only one convolution layer, limiting its feature extraction capability. 3) Simple connections between convolutional blocks hinder effective global feature fusion, causing reconstructed images to lack details. To overcome the shortcomings of residual dense network-based models, this paper addresses the problem of image restoration by proposing a novel image restoration model called the Multi-Skip Feature Sharing Residual Network (abbreviated as MSFSRNet). In MSFSRNet, the dense connections in the residual dense network are replaced with multi-skip connections to form a multi-skip feature sharing residual block (MSFSRB), which reduces the number of redundant features. Each layer in MSFSRB contains two convolutional layers, called multi-skip feature sharing convolutional layers (MSFSConv), which improves the extraction of local features in MSFSRB. In addition, a feature enhancement layer (FEL) is inserted after each MSFSRB to better integrate global features. Extensive experiments on eleven synthetic datasets and real-world datasets show that our MSFSRNet performs favorably against several state-of-the-art models on two image restoration tasks including image super-resolution and image denoising.
 </p>
 
# Experimental Datasets
## Image Denoising
###  Gray-Scale Image Denoising
* **BSD68 [1]**: BSD68 is a grayscale image converted from the CBSD68 dataset.
* **Set12 [2]**: Set12 is a collection of 12 grayscale images of different scenes that are widely used for evaluation of image denoising methods. The size of each image is 256×256.
###  Synthetic Color Image Denoising
* **CBSD68 [1]**: Color BSD68 dataset for image denoising benchmarks is part of The Berkeley Segmentation Dataset and Benchmark. It is used for measuring image denoising algorithms performance. It contains 68 images. https://github.com/clausmichele/CBSD68-dataset
* **Kodak24 [3]**: Kodak24 includes 24 color images, all images are 500*500 in size.
* **McMaster [4]**: The McMaster dataset is a dataset for color demosaicing, which contains 18 cropped images of size 500×500.
###  Real-World Color Image Denoising
* **SIDD [5]**:  SIDD includes about 30,000 noise images from 10 scenes, taken by 5 representative smartphone cameras, and generated their ground truth images. https://abdokamel.github.io/sidd/#sidd-benchmark
* **DND [6]**:  It consists of 50 pairs of real noisy images and corresponding ground truth images that were captured with consumer grade cameras of differing sensor sizes. For each pair, a reference image is taken with the base ISO level while the noisy image is taken with higher ISO and appropriately adjusted exposure time. The reference image undergoes a careful post-processing entailing small camera shift adjustment, linear intensity scaling and removal of low-frequency bias. The post-processed image serves as ground truth for our denoising benchmark. https://noise.visinf.tu-darmstadt.de/
## Image super-resolution
* **Set5 [7]**: The Set5 dataset is a dataset consisting of 5 images (“baby”, “bird”, “butterfly”, “head”, “woman”) commonly used for testing performance of Image Super-Resolution models.
* **Set14 [8]**: The Set14 dataset is a dataset consisting of 14 images commonly used for testing performance of Image Super-Resolution models.
* **BSD100 [9]**: The BSD100 dataset is a dataset consisting of 100 images commonly used for testing performance of Image Super-Resolution models.
* **Urban100 [10]**: The Urban100 dataset contains 100 images of urban scenes. It commonly used as a test set to evaluate the performance of super-resolution models.
* **Manage109 [11]**: The Manage109 dataset is a dataset consisting of 109 images commonly used for testing performance of Image Super-Resolution models.

References: <br>
[1] Julien Mairal, Francis R. Bach, Jean Ponce, Guillermo Sapiro, Andrew Zisserman: Non-local sparse models for image restoration. IEEE 12th International Conference on Computer Vision, ICCV 2009: 2272-2279. https://doi.org/10.1109/ICCV.2009.5459452 <br>
[2] Stefan Roth, Michael J. Black:Fields of Experts: A Framework for Learning Image Priors.2005 IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR 2005), 20-26 June 2005, San Diego, CA, USA.: 860-867. https://doi.org/10.1109/CVPR.2005.160 <br>
[3] Franzen R (1999) Kodak lossless true color image suite vol 4, https://r0k.us/graphics/kodak. <br>
[4] Lei Zhang, Xiaolin Wu, Antoni Buades, Xin Li: Color demosaicking by local directional interpolation and nonlocal adaptive thresholding. J. Electronic Imaging 20(2): 023016 (2011). https://doi.org/10.1117/1.3600632 <br>
[5] Abdelrahman Abdelhamed, Stephen Lin, Michael S. Brown: A High-Quality Denoising Dataset for Smartphone Cameras. Proceedings of the 2018 IEEE Conference on Computer Vision and Pattern Recognition, CVPR 2018: 1692-1700. https://doi.org/10.1109/CVPR.2018.00182 
[6] Tobias Plötz, Stefan Roth: Benchmarking Denoising Algorithms with Real Photographs. 2017 IEEE Conference on Computer Vision and Pattern Recognition, CVPR 2017: 2750-2759. https://doi.org/10.1109/CVPR.2017.294 
[7] Marco Bevilacqua, Aline Roumy, Christine Guillemot, Marie-Line Alberi-Morel:Low-Complexity Single-Image Super-Resolution based on Nonnegative Neighbor Embedding. BMVC 2012: 1-10. https://doi.org/10.5244/C.26.135 <br>
[8] Roman Zeyde, Michael Elad, Matan Protter:On Single Image Scale-Up Using Sparse-Representations. Curves and Surfaces 2010: 711-730. https://doi.org/10.1007/978-3-642-27413-8_47 <br>
[9] David R. Martin, Charless C. Fowlkes, Doron Tal, Jitendra Malik: A Database of Human Segmented Natural Images and its Application to Evaluating Segmentation Algorithms and Measuring Ecological Statistics. Proceedings of the Eighth International Conference On Computer Vision (ICCV-01), Vancouver, British Columbia, Canada, July 7-14, 2001: 416-425. https://doi.org/10.1109/ICCV.2001.937655. <br>
[10] Jia-Bin Huang, Abhishek Singh, Narendra Ahuja:Single image super-resolution from transformed self-exemplars.IEEE Conference on Computer Vision and Pattern Recognition, CVPR 2015, Boston, MA, USA, June 7-12, 2015.:5197-5206. https://doi.org/10.1109/CVPR.2015.7299156 <br>
[11] Yusuke Matsui, Kota Ito, Yuji Aramaki, Azuma Fujimoto, Toru Ogawa, Toshihiko Yamasaki, Kiyoharu Aizawa:Sketch-based manga retrieval using manga109 dataset. Multim. Tools Appl. 76(20): 21811-21838 (2017). https://doi.org/10.1007/s11042-016-4020-z. <br>
