# Installation:

The entire project was run and developed on [Google Colab](https://colab.research.google.com/) and is exported as a notebook file. Please refer to [image_captioner.ipynb](https://github.com/Prajwal-S-Venkatesh/image-captioner/blob/main/image_captioner.ipynb) for further details and insights.

> To download the dataset please vist https://cocodataset.org/#download

### Install PyTorch and Torchvision libraries
```pip install torch torchvision```

### Install Transformers library
```pip install transformers```

### Install ROUGUE score, evaluate and datasets packages
```pip install rouge_score evaluate datasets```


# Testing Framework

Although, it is important to note that testing is a crucial aspect of software development and should be incorporated into any project. I've NOT done a through testing of the model. But to test the image captioning model, a few possible test cases and scenarios could include:

- Testing the model's accuracy: Test the model with a set of images and compare the generated captions against the expected results to verify the model's accuracy.

- Testing the model's robustness: Test the model with different types of images and analyze whether the model can generate accurate captions for each type of image.

- Testing the model's efficiency: Test the model's runtime and memory usage for different sizes of images and batch sizes to ensure it can handle large-scale input and output.


# Dataset

The image data used for training and testing the image captioning model is sourced from the COCO dataset. The COCO dataset is a large-scale image recognition, segmentation, and captioning dataset containing over 330K images with 2.5 million object instances annotated with 80 object categories, and 5 captions per image.

The COCO dataset can be accessed and downloaded from the official COCO website at http://cocodataset.org/. The website provides links to download the dataset in different formats, including images, annotations, and captions. The website also provides detailed documentation and guidelines on how to use the dataset.


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

