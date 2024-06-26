# Retina-Explorer
Retina Explorer is a tool designed for exploring Eye Fundus Image Datasets using the FiftyOne visualization tool by Voxel51. It is currently hosted at https://autograd.live.

We provide a list of scripts for generating image metrics and loading data on FiftyOne. 

This project is part of anomalies detection and segmentation for Eye Fundus Images in order to grade Diabetic Retinopathy.

Currently supported datasets:
- BRSET (images + multilabel)
- DDR (images + lesion segmentation masks + metrics on connected components of segmentation masks)
- FIVES (images + vessels masks)
- DIARETDB1 (images + lesion segmentation masks + metrics on connected components of segmentation masks)

Working on support following datasets:
- IDRiD
- TJDR
- DRAC22
- MAPLES-DR

map:
/data/dataset_x/{data.csv, *}     # path for downloaded dataset
/src/loader.py                    # fiftyone dataset generic loading script: supporting grouped datasets, segmentation masks, multilabel indexing
/src/metrics/{generate_data_X.py} # generate data.csv adding more metrics if needed
/config.yaml                      # define which datasets will be loaded
