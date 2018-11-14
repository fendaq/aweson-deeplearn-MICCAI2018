# aweson-deeplearn-MICCAI2018

## Paper list

### [1.](#VoxelAtlasGAN) [VoxelAtlasGAN: 3D Left Ventricle Segmentation on Echocardiography with Atlas Guided Generation and Voxel-to-Voxel Discrimination](http://cn.arxiv.org/abs/1806.03619)

### [2.](#Self-paly) [Generalizing Deep Models for Ultrasound Image Segmentation](https://www.researchgate.net/publication/327629404_Generalizing_Deep_Models_for_Ultrasound_Image_Segmentation_21st_International_Conference_Granada_Spain_September_16-20_2018_Proceedings_Part_IV)


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
   

### Self-paly deep model
Generalizing Deep Models for Ultrasound Image Segmentation
 -School : 深圳大学，香港中文大学
 -Disease : None
 -Tasks : segment congeneric prenatal ultrasound images
 -Challenge : retrain when 



