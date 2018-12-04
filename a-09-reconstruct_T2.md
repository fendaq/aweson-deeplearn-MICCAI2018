## Ultra-Fast T2-Weighted MR Reconstruction Using Complementary T1-Weighted Information

### Challenge
The total acquisition time of ~10 min yields the image quality vunerable to artifacts such as motion

### Task
speed up the reconstruction
```
                        reconstruct          
T1 + under-sampled T2 --------------> fully-sampled T2    
```

DL : Dense-Unet, signal-noise-ratio(SNR) loss, mean squared error(MSE)

### MRI advantages and disadvantage
1. better measure different soft tissue contrasts

2. avoids exposing patients to harmful ionizing radiation

3. limit acquisition speed

### T1 and T2
```
T1 (1) assess the cerebral cortex
   (2) identifying fatty issue
   (3) characterize focal liver lesions
   (4) obtain morphological information, post-contrast imaging
   
T2 (1) detect edema and inflammation
   (2) reveal white matter lesions
   (3) assess zonal antomy in the prostate and uterus
```
### Pre-process steps
```
1. denoise with the NL-means
2. rigid registration
3. brain extraction, vloBrain
4. bias correction, N4 algorithm
5. intensity normalization to (0,1)
```
### Interesting
they demonstrated to learn the spatitemporal correlation efficiency by leveraging convolution
and data sharing layers together
   
