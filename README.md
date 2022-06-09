# STPSR
We propose a structure and texture preserving network (STPSR) for real-world image super-resolution, which extracts both structural information and local textures.

<p align="center">  
  <img src="https://github.com/bjzzhou/STPSR/blob/main/Figures/framework.png">  
</p>


## Quantitative Results
Our work in this direction focuses more on perceptual quality, and non-reference image quality evaluation (NIQE) is seen as the main metric after Real-ESRGAN, with lower NIQE values indicating higher perceptual quality.

Table1. NIQE scores on several diverse testing datasets with real-world images. The scale factors is x4. The best result is highlighted in red.
<img src="https://github.com/bjzzhou/STPSR/blob/main/Figures/table1.png"> 

We compare the performance on six benchmark datasets with our backbone method Real-ESRGAN.

Table2. Average PSNR/SSIM values for scale factors x4 on synthetic datasets.

<img src="https://github.com/bjzzhou/STPSR/blob/main/Figures/table2.png">  

    
## Qualitative Results
### On real-world datasets

<p align="center">  
  <img src="https://github.com/bjzzhou/STPSR/blob/main/Figures/other_real.png">  
</p>

### On synthetic datasets
Visual results between Real-ESRGAN and our method. The examples are from datasets BSD100, Urban100, and DIV2K validation. The scale factor is x4.

<p align="center">  
  <img src="https://github.com/bjzzhou/STPSR/blob/main/Figures/other_synthetic.png">  
</p>

## Acknowledgement
Our implementation of STPSR is based on the [BasicSR](https://github.com/XPixelGroup/BasicSR) and [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN).
