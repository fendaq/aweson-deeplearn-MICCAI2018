# aweson-deeplearn-MICCAI2018

## Paper list

### [a1.](#VoxelAtlasGAN) [VoxelAtlasGAN: 3D Left Ventricle Segmentation on Echocardiography with Atlas Guided Generation and Voxel-to-Voxel Discrimination](http://cn.arxiv.org/abs/1806.03619)

### [a2.](#Self-play) [Generalizing Deep Models for Ultrasound Image Segmentation](https://www.researchgate.net/publication/327629404_Generalizing_Deep_Models_for_Ultrasound_Image_Segmentation_21st_International_Conference_Granada_Spain_September_16-20_2018_Proceedings_Part_IV)

### [a3.](#ASD-Net) [ASDNet: Attention Based Semi-supervised Deep Networks for Medical Image Segmentation](https://link.springer.com/content/pdf/10.1007%2F978-3-030-00937-3_43.pdf) (Impressive)

### [a4.](#Multi-task)[Deep Adversarial Context-Aware Landmark Detection for Ultrasound Imaging](https://www.researchgate.net/publication/325413928_Deep_Adversarial_Context-Aware_Landmark_Detection_for_Ultrasound_Imaging)

### [b1.](#Cosine) [Instance Segmentation and Tracking with Cosine Embeddings and Recurrent Hourglass Networks](https://arxiv.org/abs/1806.02070)

### [b2.](#SLSDeep) [SLSDeep: Skin Lesion Segmentation Based on Dilated Residual and Pyramid Pooling Networks](https://www.researchgate.net/publication/325396517_SLSDeep_Skin_Lesion_Segmentation_Based_on_Dilated_Residual_and_Pyramid_Pooling_Networks)

### [c1.](#Deformable) [A Discriminatively Trained, Multiscale, Deformable Part Model](https://www.researchgate.net/publication/221363206_A_Discriminatively_Trained_Multiscale_Deformable_Part_Model)

## Paper content

### VoxelAtlasGAN
VoxelAtlasGAN: 3D Left Ventricle Segmentation on Echocardiography with Atlas Guided Generation and Voxel-to-Voxel Discrimination
 
 - School : 哈工大、哈尔滨第四医科大学、werstern university
 - Diseases : cardiac disease(心脏病)
 - Tasks : 3D left ventricle(LV) segmentation on echocardiography
 - Challenge : lower contrast,higher noise, data dimensionality, limited annotation of 3D echocardiography
 - Contributions :
   - voxel-to-voxel cGAN
   - embeds the 3D LV atlas into an end-to-end optimization framework
   - traditional discrimination loss + new proposed consistent constraint
 - Evaluation methods:
   - mean surface distance
   - mean hausdorff surface distance
   - mean dice
   - correlation of EF
   - mean inference speed
 - **Intersting :** 
   - Atlas guided generation
   - Consistent constraint, including of segmentation consistent constraint and vlume consistent constraint
   

### Self-play
Generalizing Deep Models for Ultrasound Image Segmentation

 - School : 深圳大学，香港中文大学
 - Disease : None
 - Tasks : segment congeneric prenatal ultrasound images
 - Challenge : retrain required when new corpus otherwise performance drop
 - Contributions :
   - single img from target corpus needed, without modeling ppearance conversion in advance
   - Self-play training strategy to pre-train
   - Composite appearance and structure constraints
 - Evaluation : seven matrics
   - Dice coefficient (DSC)
   - Conformity (Conf)
   - Hausdorff distance of Boundaries(Hdb)
   - Average distance of boundaries(Adb)
   - Precision
   - Recall
 - **Interesting**
   - Corpus-level conversion models can match the appearance distributions of different corpora from a global perspective
   - auxiliary supervision and skip connection

### ASD-Net
ASDNet: Attention Based Semi-supervised Deep Networks for Medical Image Segmentation

- School : University of North Carolina at Chapel Hill （北卡罗纳）
- Tasks : Pelvic organ segmentation (骨盆器官分割)
- Challenge : relieve the demand for large-scale labeled data
- Contributions :
  - multi-class dice loss
  - regien-attention based semi-supervised learning strategy
- Meaning : biopsy and cancer radiation therapy (活组织检测)
- Difficulties in acquiring training set:
  - manual annotation requires expertise knowledge
  - pixel-wise(voxel-wise) label maps is time-consuming
  - suffers from large intra- and inter- observer variability
- Evaluation :
  - Dice Score Coefficiency(DSC)
  - Average Surface Distance(ASD)
- Remaining :
  - focal loss

### Cosine
Instance Segmentation and Tracking with Cosine Embeddings and Recurrent Hourglass Networks

- School : Graz University of Technology, Austria
- Tasks : 
  - Left ventricles in MR videos
  - Cell instance segmentation
  - ISBI cell tracking challenge
- Challenge : others solely segment one instance at a time
- Contributions :
  - First temporal information for tracking instance segmentation
  - cosine embedding loss
- Evaluation : intersection over union(IOU)
- **Intersting :** data augmentation with SimpleITK

### SLSDeep
SLSDeep: Skin Lesion Segmentation Based on Dilated Residual and Pyramid Pooling Networks

- School : 罗维拉-威尔吉利大学
- Task : skin lesion segmentation(SLS)
- Disease : melanoma
- Challenge : 
  - dermoscopic images has various characteristics including different sized and shapes, fuzzy boundaries, different
    colors, and the presence of hair
  - Since the melanoma is mostly a small part of a dermoscopic image, the minimization of cross-entropy tends to be **biased** towards the background
- Contributions :
  - dilated residual + pyramid pooling networks
  - loss function = Negative Log Likelihood(NLL) + End Point Error(EPE)
- Evaluation : accuracy, Dice coefficient, Jaccard index, specificity
- Interesting :
  - the best results were provided when only one skip connection was done between the last layer of the encoder and the output
  of PPN layer of the decoder
  
### Multi-task
Deep Adversarial Context-Aware Landmark Detection for Ultrasound Imaging

- School : 帝国理工大学 Imperial College London
- Task : prostate gland localization within the ultrasound image in real-time
- Challenge :
  - low tissue contrast
    - fuzzy boundaries
    - varing prostate gland sizes
  - inherent label noise, signal droupout
  - robust localization of prostate landmarks
- Contributions :
  - a new deep learning based approach, localizing several prostate landmarks efficiently and robustly
  - a multi-task learning approach, more contextually aware
  - dicriminator adds to motivate that the boundary is a smooth closed shape (增加约束)
  
- Intersting : Conditional Random Fields, **trans-rectal ultrasound images**, 


### Deformable
A Discriminatively Trained, Multiscale, Deformable Part Model

- School : 芝加哥大学
- Contributions :
  -- deformable parts
  -- discriminative training, latent SVM
- Experiment
