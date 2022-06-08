# STPSR
We propose a structure and texture preserving network (STPSR) for real-world image super-resolution, which extracts both structural information and local textures.

<p align="center">  
  <img src="https://github.com/bjzzhou/STPSR/blob/main/Figures/framework.png">  
</p>


## Quantitative Results
Our work in this direction focuses more on perceptual quality, and non-reference image quality evaluation (NIQE) is seen as the main metric after Real-ESRGAN, with lower NIQE values indicating higher perceptual quality.

Table1. NIQE scores on several diverse testing datasets with real-world images.

| Datasets | Bicubic | ESRGAN | DAN | RealSR | BSRGAN | Real-ESRGAN | Ours |
| -------- | ------- | ------ |---- | ------ | ------ | ----------- | ---  |
| DPED | 6.0121 | 5.7363 | 6.1414 | 5.5855 | 5.9906 | 4.3784 | $\color{red}{4.2126}$ |
| RealSR-Canon | 6.1269 | 6.7715 | 6.5282 | 6.8692 | 5.7489 | 4.0360 | $\color{red}{3.8547}$
| RealSR-Nikon | 6.3607 | 6.7480 | 6.6063 | 6.7390 | 5.9920 | 4.4656 | $\color{red}{4.2406}$
| OST300 | 4.4440 | 3.5245 | 5.0232 | 4.5715 | 4.1662 | $\color{red}{2.6395}$ | 2.7755
| ADE20K_val | 7.5239 | 3.6905 | 6.3839 | 3.4102 | 3.9434 | 3.3156 | $\color{red}{3.2887}$

Table2. Average PSNR/SSIM values for scale factors x4 on synthetic datasets.

|            | Real-ESRGAN | Ours | | |
| ---------- | ---------- | ---------- | ---------- | ---------- |
| | PSNR | SSIM | RSNR | SSIM |
| Set5       | 25.756 | 0.7910 | **27.179** | **0.8091**
| Set14      | 24.831 | 0.6826 | **25.536** | **0.6875**
| Urban100   | 22.166 | 0.6724 | **23.076** | **0.6867**
| BSD100     | 24.517 | 0.6305 | **24.995** | **0.6337**
| General100 | 26.544 | 0.7684 | **27.352** | **0.7776**
| DIV2K val  | 25.961 | 0.7396 | **26.743** | **0.7458**
    
    
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

## Ablation Study
We conduct ablation studies to investigate the roles of major components in our method, including local loss and ST branch. 
