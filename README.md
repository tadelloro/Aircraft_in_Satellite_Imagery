## Aircraft in Satellite Imagery

#### Problem
Satellite images collected over airports and other areas in California are processed for modeling and analysis. Initial data exploration is performed including data visualization and hypothesis tests. Binary classifiers are then trained to label each satellite image as containing a plane or not containing a plane. Five machine learning models (i.e., Logistic Regression, K-Nearest Neighbors, Random Forest, SVM, and Gradient Boosting) and two Convolutional Neural Networks are trained and tested to detect planes in a dataset of 32,000 satellite image chips collected over California.

#### Business Case
Automated analysis and classification of satellite imagery has various real world applications in industries such as agriculture, defense, intelligence, energy, and/or finance. 

#### Jupyter Notebooks
* Stage 1 includes exploratory data analysis and bootstrap hypothesis testing.
* Stage 2 includes modeling and performance results.

#### Datasets
The PlanesNet data are available in the Kaggle dataset “Planes in Satellite Imagery”, provided by Planet Labs Inc. The data are 20x20 images, each with three bands, in a JSON formatted file containing data, labels, scene id's, and location metadata. A total of 32,000 images are provided, the total JSON file size is 191 Mb. Satellite imagery used to build PlanesNet is made available through Planet Labs' Open California dataset, which is openly licensed.

The Kaggle dataset can be found here:
* https://www.kaggle.com/rhammell/planesnet#planesnet.json


| JSON formatted text file | Description                                                                                                                   |
|--------------------------|-------------------------------------------------------------------------------------------------------------------------------|
| data                     | Pixel value data for each 20x20 RGB image is stored as a list of 1200 integers. The first 400 for red, then green, then blue. |
| label                    | Valued 1 or 0, representing the "plane" class and "not-plane" class, respectively.                                            |
| scene id                 | The unique identifier of the PlanetScope visual scene the image chip was extracted from.                                      |
| longitude & latitude     | The longitude and latitude coordinates of the image center point, with values separated by a single underscore.               |


