## A Framework for Identifying Diabetic Retinopathy Based on Anti-noise Detection and Attention-Based Fusion

inputs : DR grades and bounding boxes of MA and HE lesions

We :  
  - detecion model, extract lesion information into a lesion map
  - fuse it with the orighinal image for DR identification
  
(1) anti-noise Center-Sample Modeule : predicts the probabilities of the lesions in the entire image

(2) Attension Fusion Network(AFN) : identify DR grades, learn weights between the original images and lesion maps

### Datasets
EyePACS, Messidor

### Center-Sample detector
(1) shared deature extractor

(2) clssification/bounding box detecting header

(3) Noisy sample Mining module
  - sample clustering
  - Noisy Sample Mining : determing the noisy samples and reducing their sampling weight

(1) + (2) : lesion probablity map

### Attension Fusion Network
two feature extractors + an attension network

### Evaluation
quadratic weighted kappa score, AUC
