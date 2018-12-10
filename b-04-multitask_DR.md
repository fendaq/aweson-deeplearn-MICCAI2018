## A Multitask Learning Architecture for Simultaneous Segmentation of Bright and Red Lesions in Fundus Images

we extent U-net on multi-task learning, single encoding module, multiple decoding modules

kappa-based function loss

### Advantages
shorter inference times, train a single architecture perfomr multiple highly specialized tasks thath share a common basis

CRFs \[10] \[11]

### Data augmentation
geometrical : translation, rotation, shearing, elastic distortion

color : brightness, contrast, gamma, HSV saturation/value

### Dataset
DIARETDB1
