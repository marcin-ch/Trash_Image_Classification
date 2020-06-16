# Trash Image Classification
## Overview
Project's goal is to train as simple as possible CNN (Convolutional Neural Network) for classifying images of trash (32x32) into one of the categories:
* cardboard
* glass
* metal
* paper
* plastic
* trash

Project has been created as Jupyter notebook hosted by Google Colaboratory (or Colab for short). Colab allows you to write and execute Python in your browser with zero configuration required, free access to GPUs and easy sharing (more info [here](https://colab.research.google.com/notebooks/intro.ipynb)).

## Notebooks explanation
* *Trash_Image_Classification.ipynb* - contains dataset uploading, image preprocessing, model creation, model training, making and verifying predictions. Finally, trained model is saved in HDF5 format (.h5).<br>
To open this notebook hit bellow button and then `Runtime -> Run All` (you must be logged in with a Google Account to continue):<br>
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/marcin-ch/Trash_Image_Classification/blob/master/Trash_Image_Classification.ipynb)

* *Test_Trash_Image_Classification.ipynb* - created to test loading of the saved model and making predictions using this model.<br>
To open this notebook hit bellow button and then `Runtime -> Run All` (you must be logged in with a Google Account to continue):<br>
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/marcin-ch/Trash_Image_Classification/blob/master/Test_Trash_Image_Classification.ipynb)

## Saved model
* *trash_image_classification.h5* - achieved accuracy on training images is 88%, on testing images is 64%.

## Dataset
Dataset comes from:
https://github.com/garythung/trashnet/blob/master/data/dataset-resized.zip

Changes:
1. Names of the images changed (added underscore between the core name and number), e.g.
* *cardboard1.jpg* to *cardboard_1.jpg*,
* *glass2.jpg* to *glass_2.jpg* and so on
> Used *IrfanView* (`File -> Batch Conversion/Rename`)
2. All images moved to one folder (2527 in total):
* from folder *cardboard* (403 files),
* from folder *glass* (501 files),
* from folder *metal* (410 files),
* from folder *paper* (594 files),
* from folder *plastic* (482 files),
* from folder *trash* (137 files)
3. All images splitted into two folders: *train* and *test*, 80% images goes to *train* folder and 20% goes to *test* folder (images chosen randomly, manually)

Category | Train | Test | SUM
--- | --- | --- | ---
cardboard | 323 | 80 | 403
glass | 401 | 100 | 501
metal | 330 | 80 | 410
paper | 476 | 118 | 594
plastic | 386 | 96 | 482
trash | 110 | 27 | 137
***total*** | ***2026*** | ***501*** | ***2527***

4. Zipped and upload to Github as *dataset_trash.zip*
