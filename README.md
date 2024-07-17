# Semantic segmentation model for voids in irradiated Ni metal

This package is developed to perform semantic segmentation of voids in Ni metal irradiated by krypton ions using IVEM at ANL.

## Segmentation models
The semantic segmentation models trained in this work are based on the package [segmentation_models.pytorch](https://github.com/qubvel-org/segmentation_models.pytorch). By mixing different segmentation model, encoder, loss function and batch size, more than 100 different segmentation models were trained and tested. Using the top-15 segmentation models, an ensemble method was created using soft voting classifier for individual pixels in each image. More details regarding the segmentation models can be found in our [publication](https://www.sciencedirect.com/science/article/pii/S1359645423003440?via%3Dihub).

The semantic microstructure segmentation dataset consists of 204 manually annotated TEM images of krypton-ion-irradiated Ni at different irradiation conditions, e.g., temperatures and doses and imaging conditions, e.g., magnification, diffraction contrast, and defocus. Some of the images can be found in the folder test.

## Installation

The environment can be installed via Anaconda: ``conda env create --file environment.yml --force``

## Run segmentation model

A jupyter notebook was included to run the voids segmentation model. Due to the size limit, the trained models can be downloaded from the link here.

Folders test and testannot are the examples of the original TEM images and annotated binary mask files for the corresponding TEM images, which can be used to evaluate the model performance using the included ground truth annotations.

## Support

This material is based upon work supported by Laboratory Directed Research and Development (LDRD) funding from Argonne National Laboratory, provided by the Director, Office of Science, of the U.S. Department of Energy under Contract No. DE-AC02-06CH11357.

The folder new_images_Sep_2022 includes a few example images used to predict the voids using the current semantic segmentation models.
