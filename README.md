# Retina-Explorer
Retina Explorer is a tool designed for researchers to explore Eye Fundus Image Datasets and query its metrics seamlessly.
It was made using Python, OpenCV and FiftyOne visualization tool by Voxel51.

## Installation

## Usage
### Download datasets

### Configure which datasets to load

### Run FiftyOne



## Currently implemented datasets:
- BRSET (images + multilabel)
- DDR (images + lesion segmentation masks + metrics on connected components of segmentation masks)
- FIVES (images + vessels masks + vessels metrics)
- DIARETDB1 (images + lesion segmentation masks + metrics on connected components of segmentation masks)

--- 

Feel free to use our code as base/inspiration to adapt to your own dataset, metrics and research.

map:
/data/dataset_x/{data.csv, *}     # path for downloaded dataset
/src/loader.py                    # fiftyone dataset generic loading script: supporting grouped datasets, segmentation masks, multilabel indexing
/src/metrics/{generate_data_X.py} # generate data.csv adding more metrics if needed

/config.yaml                      # define which datasets will be loaded
