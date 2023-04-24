# UMLS augmented biomedical-ner and relationship-classification model

This project contains code for training and evaluating various named entity recognition (NER) and relation extraction models.

## File Structure

The file structure of this project is as follows:

- `data`: This directory contains the annotation guidelines in the `ADE_Annotation_Guideline_final.pdf` file.
- `notebooks`: This directory contains all Jupyter notebooks used in the project.
    - `data_prep`: This directory contains notebooks used for preparing the data for training the models.
        - `data-parser.ipynb`: This notebook contains code for parsing the raw data files.
        - `data-prep-baseline.ipynb`: This notebook contains code for preparing the data for training the baseline NER model.
        - `data-prep-flair.ipynb`: This notebook contains code for preparing the data for training the Flair-based NER model.
        - `umls-data-augmentation.ipynb`: This notebook contains code for augmenting the training data using UMLS concepts.
    - `models`: This directory contains notebooks used for training the models.
        - `ner`: This directory contains notebooks used for training the NER models.
            - `baseline`: This directory contains notebooks used for training the baseline NER model.
                - `ner-baseline.ipynb`: This notebook contains code for training the baseline NER model.
            - `lstm-crf`: This directory contains notebooks used for training the LSTM-CRF NER models.
                - `ner-lstm-crf.ipynb`: This notebook contains code for training the LSTM-CRF NER model.
                - `ner-lstm-crf-umls-augmented.ipynb`: This notebook contains code for training the LSTM-CRF NER model with UMLS-augmented data.
                - `ner-lstm-crf-umls-augmented-weight_exp.ipynb`: This notebook contains code for training the LSTM-CRF NER model with UMLS-augmented data and weight experimentation.
            - `transformer-crf`: This directory contains notebooks used for training the Transformer-CRF NER models.
                - `ner-transformer-crf.ipynb`: This notebook contains code for training the Transformer-CRF NER model.
                - `ner-transformer-crf-augmented.ipynb`: This notebook contains code for training the Transformer-CRF NER model with UMLS-augmented data.
                - `ner-transformer-crf-augmented-weight_exp.ipynb`: This notebook contains code for training the Transformer-CRF NER model with UMLS-augmented data and weight experimentation.
        - `relation_extractor`: This directory contains notebooks used for training the relation extraction models.
            - `rel-baseline.ipynb`: This notebook contains code for training the baseline relation extraction model.
            - `rel-flair.ipynb`: This notebook contains code for training the Flair-based relation extraction model.
- `README.md`: This file, containing the project overview and file structure.

## Usage

Clone this repository and run the Jupyter notebooks in the order specified by their directory names. Note that some notebooks may require additional dependencies, which can be installed using the provided `requirements.txt` file.

