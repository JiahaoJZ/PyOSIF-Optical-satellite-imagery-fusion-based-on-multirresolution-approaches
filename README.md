# Satellite images fusion

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

## 1. Description
This repository implements **pansharpening** and **multispectral images fusion** algorithms based on the wavelet transform calculated by the à trous algorithm, using Python. The images used are downloaded from [Google Earth Engine](https://developers.google.com/earth-engine/datasets/), **pansharpening** is applied to [Landsat 8 raw images](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C01_T1), and **multispectral images fusion** is performed over [Landsat 8 surface reflectance images](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C01_T1_SR) and [Sentinel 2 surface reflectance images](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR).

## 2. Usage
To execute the [jupyter notebooks](https://jupyter.org/), an environment including the dependencies is offered. This environment can be found in [image_fusion.yml](https://github.com/JiahaoJZ/Image_fusion/blob/master/image_fusion.yml).
After importing the environment in [conda](https://www.anaconda.com/). You can proceed with the execution of the notebooks.

There are 2 main execution flows:

  - **Pansharpening**:
To perform pansharpening, download the Landsat 8 images using [Download_Landsat8_Images.ipynb](https://github.com/JiahaoJZ/Image_fusion/blob/master/Download_Landsat8_Images.ipynb) (A Google Earth Engine validated account is requiered), and then use [Pansharpening.ipynb](https://github.com/JiahaoJZ/Image_fusion/blob/master/Pansharpening.ipynb), to fuse the multispectral and the panchromatic image.

  - **Multispectral images fusion**:
To perform multispectral images fusion, download the Landsat 8 and Sentinel 2 images using [Download_Landsat8_and_Sentinel2_Images.ipynb](https://github.com/JiahaoJZ/Image_fusion/blob/master/Download_Landsat8_and_Sentinel2_Images.ipynb), then use [Resizing_Module.ipynb](https://github.com/JiahaoJZ/Image_fusion/blob/master/Resizing_Module.ipynb) to resize the Landsat 8 image to the Sentinel 2 image pixel size. Finally, you can do the multispectral images fusion executing [Multispectral_Images_Fusion.ipynb](https://github.com/JiahaoJZ/Image_fusion/blob/master/Multispectral_Images_Fusion.ipynb).
