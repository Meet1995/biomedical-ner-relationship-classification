# UMLS augmented biomedical-ner and relationship-classification model

This repository contains code and data for a natural language processing project. The project includes notebooks for experiments on data parsing, preprocessing, named entity recognition (NER), and relation extraction (REL). The code is organized into the following directory structure:

- `data`: This directory contains the data used in the project, including an annotation guideline and a README file.
    - `ADE_Annotation_Guideline_final.pdf`: This is a PDF file containing the annotation guideline for the project. It describes how the data was annotated and provides instructions for annotating new data.

- `notebooks`: This directory contains Jupyter notebooks for running the experiments. It includes a subdirectory called `experiments`, which contains the notebooks organized by task. Here are brief descriptions of the notebooks:
    - `data-parser.ipynb`: This notebook is used to parse the data used in the project. It includes code for cleaning, normalizing, and transforming the data into a format that can be used in downstream tasks.
    - `data-prep-baseline.ipynb`: This notebook is used to prepare the data for use in a baseline NER model. It includes code for splitting the data into training and testing sets, generating features for the model, and performing other preprocessing steps.
    - `data-prep-flair.ipynb`: This notebook is used to prepare the data for use in a NER model that uses Flair embeddings. It includes code for generating embeddings, splitting the data, and performing other preprocessing steps.
    - `ner-baseline.ipynb`: This notebook is used to train and evaluate a baseline NER model. It includes code for initializing the model, training it on the training data, and evaluating its performance on the testing data.
    - `ner-lstm-crf.ipynb`: This notebook is used to train and evaluate a NER model that uses an LSTM-CRF architecture. It includes code for initializing the model, training it on the training data, and evaluating its performance on the testing data.
    - `ner-transformer-crf.ipynb`: This notebook is used to train and evaluate a NER model that uses a Transformer-CRF architecture. It includes code for initializing the model, training it on the training data, and evaluating its performance on the testing data.
    - `preprocessing.ipynb`: This notebook is used to perform general preprocessing on the data. It includes code for tokenizing the text, converting it to lowercase, and removing stop words.
    - `rel-baseline.ipynb`: This notebook is used to train and evaluate a baseline REL model. It includes code for initializing the model, training it on the training data, and evaluating its performance on the testing data.
    - `rel-flair-embeddings.ipynb`: This notebook is used to train and evaluate a REL model that uses Flair embeddings. It includes code for generating embeddings, initializing the model, training it on the training data, and evaluating its performance on the testing data.