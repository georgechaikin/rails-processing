# rails-processing
Scripts for rails preprocessing and detection using segmentation model
# Requirements
See [requirements.txt](https://github.com/georgechaikin/rails-processing/blob/main/requirements.txt)
# How it works
There were several steps to train the model:
1. 30 images were labeled manually to train the model with pretrained backbone (with random zoom and random rotation)
2. The scripts for labels convertion (to CVAT format and from CVAT format) prepared
3. All train sample images were labeled using the model, then the mistakes were manually corrected (especially false-positive mistakes)
4. The model was trained again using all train data
# Source code
You can see the code for U-Net outputs in [rails-train.ipynb](https://github.com/georgechaikin/rails-processing/blob/main/rails-train.ipynb)
