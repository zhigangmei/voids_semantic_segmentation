# voids_semantic_segmentation
Semantic segmentation model voids in irradiated Ni metal

Soft ensemble of 15 segmentation models trained with 129 images of voids in Kr+ ion irradiated Ni metal

The python environment for the model can be installed using the attached yaml file: environment.yml

The test images are included in the folder tests.

A jupyter notebook was included to run the voids segmentation model. Due to the size limit, the trained models can be downloaded from the link here.

Folders test and testannot are the examples of the original TEM images and annotated binary mask files for the corresponding TEM images, which can be used to evaluate the model performance using the included ground truth annotations.

The folder new_images_Sep_2022 includes a few example images used to predict the voids using the current semantic segmentation models.
