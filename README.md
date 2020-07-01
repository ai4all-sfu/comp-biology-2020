# Computational Biology Project 2020

## Topic: COVID-19 classification from microscopy cell images
### Mentors: Raquel Aoki, Janaki Sathish

[One slide Description](https://docs.google.com/presentation/d/1rDsnvqHS2EoZfHlRDT-YqbMqoBwtCkxAJzzJ2WwDxxg/edit?usp=sharing)
 
### Dataset 

Name: RxRx19

Description: Two kinds of cells are taken into consideration: Human Renal Cortical Epithelial Cells(HRCE) cells and Vero cells. Vero cells are derived from the kidney of an African green monkey. The main ‘images’ folder contains four sets of cells: HRCE-1, HRCE-2, Vero-1, Vero-2; each containing cell images for 26 Plates; each Plate folder containing 26,800 images; Each cell is stained with 5 different stains (channels) which makes it 5,359 images per channel.  Each image is 1024 x 1024 x 1. The metadata can be found in 'metadata.pkl'. The deep learning embeddings can be found in 'embeddings.pkl'. Each row in the pkl has a 'site_id' as described in the metadata schema. The remaining 1024 columns is the embedding for that respective site.

### Tasks
The directory 'notebooks' contain the code and exercises for each day of week 2. The details are as follows:

Day 1: Introduction to the dataset, hands-on experience with manipulating the metadata and deep learning embeddings of the cell images in RxRx19, feature extraction from images using basic Computer Vision techniques.

Day 2: Dimensionality reduction techniques are used in the embeddings data. The goal is find a representation of the data in a lower dimention. The factor models explored were Principal Component Analysis, Matrix Factorization and Autoencoders. 

Day 3: The feature set derived from Day 2 is used to train classification models, namely Logistic Regression, KNN Classifier, and Random Forest Classifier. This is followed by an introduction to a simple Convolutional Neural Network, which is trained using the feature embeddings and labels as well to predict if the cell image belongs to 'active' or 'inactive' class. Finally, a detailed comparison between all the four methods are made.

Day 4: Doubt sessions regarding concepts and exercises worked on during the previous days, and preparation for the presentation on Day 5. 

### References:

Heiser, Katie, et al. "Identification of potential treatments for COVID-19 through artificial intelligence-enabled phenomic analysis of human cells infected with SARS-CoV-2." bioRxiv (2020) ([link](https://www.biorxiv.org/content/10.1101/2020.04.21.054387v1.full.pdf)).

RxRx19: The First Morphological Imaging Dataset on SARS-CoV-2 Virus ([link](https://www.rxrx.ai/rxrx19))

RxRx19a COVID-19 Image Embeddings ([link](https://www.kaggle.com/tunguz/rxrx19a))

Techniques to extract features from images ([link](https://www.analyticsvidhya.com/blog/2019/08/3-techniques-extract-features-from-image-data-machine-learning-python/))

Edge detection in python ([link](https://towardsdatascience.com/edge-detection-in-python-a3c263a13e03))

