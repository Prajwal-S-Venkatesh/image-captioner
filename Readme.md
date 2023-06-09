# Final Project - Spring 2023 Big Data Technologies (CSP-554-03)

> Course taught by [Prof. Jawahar Panchal](https://www.iit.edu/directory/people/jawahar-panchal)

The Neural Image Caption Generation with Visual Attention project aims to implement a Neural Image Capton Generaton model with Visual Atention using PyTorch. Image captioning is the task of generating natural language descriptions of images, and it has a wide range of applications, from assistive technology to automated content creation. While traditional image captioning models generate captions without considering which parts of the image are relevant to the generated caption, a recent innovation in this field has led to the development of visual attention mechanisms, which enable models to focus on important parts of the image while generating captions. In this project, I’ve used the COCO (Common Objects in COntext) dataset to train an encoder-decoder model with visual attention. The project aims to investigate the development of an image captioning model using state-of-the-art deep learning techniques using PyTorch and Transformers in Python. The model uses a pre-trained image encoder to extract image features and a pre-trained language decoder to generate captions. The image encoder and language decoder are connected using a visual attention mechanism that allows the decoder to focus on different parts of the image while generating the caption.

# Installation:

The entire project was run and developed on [Google Colab](https://colab.research.google.com/) and is exported as a notebook file. Please refer to [image_captioner.ipynb](https://github.com/Prajwal-S-Venkatesh/image-captioner/blob/main/image_captioner.ipynb) for further details and insights. Download the notebook and run locally or import the notebook on GColab and run all code snippets. (NOTE: this entire notebook can take more than 10 Hrs to completely run and finish execution)

> To download the dataset please vist https://cocodataset.org/#download

### Install PyTorch and Torchvision libraries
```pip install torch torchvision```

### Install Transformers library
```pip install transformers```

### Install ROUGUE score, evaluate and datasets packages
```pip install rouge_score evaluate datasets```


# Testing Framework

Although, I've NOT done a thorough testing of the model, I've implemented a few possible test cases and scenarios that include:

- Testing the model's accuracy: Tested the model with a set of images and compared the generated captions against the expected results to verify the model's accuracy.

- Testing the model's robustness: Tested the model with different types of images and analyze whether the model can generate accurate captions for each type of image.

- Testing the model's efficiency: Tested the model's runtime and memory usage for different sizes of images and batch sizes to ensure it can handle large-scale input and output.


# Dataset

The image data used for training and testing the image captioning model is sourced from the COCO dataset. The COCO dataset is a large-scale image recognition, segmentation, and captioning dataset containing over 330K images with 2.5 million object instances annotated with 80 object categories, and 5 captions per image.

The COCO dataset can be accessed and downloaded from the official COCO website at http://cocodataset.org/. The site provides links to download the dataset in various formats, including images, annotations, and captions.


# Code Overview:

Here is a brief overview of the code:

1. Loading the COCO dataset using the PyTorch DataLoader.
2. Preprocessing the image data using PyTorch's pre-trained ResNet50 model to extract features.
3. Using the HF Transformers library to build and train the image captioning model.
4. Evaluating the model's performance using the BLEU-4 metric, which measures the similarity between the generated captions and the ground truth captions.
5. Generating captions for new images using the trained model.
6. The code requires the following dependencies:

**PyTorch:** a popular open-source machine learning library for Python.

**Transformers:** a library for natural language processing that provides easy-to-use interfaces for a wide range of pre-trained models.

**COCO API:** a Python implementation of the COCO dataset that provides tools for working with the dataset.

All of these dependencies are open-source and can be installed using pip, a package manager for Python.

The code also includes detailed documentation and comments to explain each section of the code. 

