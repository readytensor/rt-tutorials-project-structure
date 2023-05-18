# Adaptable Machine Learning Models - Tutorial 1: Project Structure

## Project Description

This repository contains the project structure defined in the first tutorial in the series on developing adaptable machine learning models. This tutorial covers the topic of creating standardized project templates for machine learning models.

This is an empty project structure that can be used as a template for any machine learning project. In the tutorial series, this project structure is used to develop a machine learning model for the binary classification task.

## Project Structure

```bash
├── examples/
├── inputs/
│   ├── data/
│   │   ├── testing/
│   │   └── training/
│   └── schema/
├── model/
│   └── artifacts/
├── outputs/
│   ├── hpt_outputs/
│   ├── logs/
│   └── predictions/
├── src/
│   ├── config/
│   ├── data_model/
│   ├── hyperparameter_tuning/
│   ├── prediction/
│   ├── preprocessing/
│   ├── schema/
│   └── xai/
├── tests/
│   ├── <mirrors `/src` structure ...>
│   ...
│   ...
├── tmp/
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

- **`/examples`**: This directory contains all files you want to use as examples. Typically, these would be small data files that can be used as examples for the ML project. We have included the titanic dataset files in this directory. This dataset is used in the tutorial series to develop a binary classification model.
- **`/inputs`**: This directory contains all the input files for your project, including the data and schema files. The data is further divided into testing and training subsets.
- **`/model/artifacts`**: This directory is used to store the model artifacts, such as trained models and their parameters.
- **`/outputs`**: The outputs directory contains all output files, including the prediction results, logs, and hyperparameter tuning outputs.
- **`/src`**: This directory holds the source code for the project. It is further divided into various subdirectories such as `config` for configuration files, `data_model` for data models for input validation, `hyperparameter_tuning` for hyperparameter-tuning (HPT) related files, `prediction` for prediction model scripts, `preprocessing` for data preprocessing scripts, `schema` for schema scripts, and `xai` for explainable AI scripts.
- **`/tests`**: This directory contains all the tests for the project. It mirrors the `src` directory structure for consistency. There is also a `test_resources` folder inside `/tests` which can contain any resources needed for the tests (e.g. sample data files).
- **`/tmp`**: This directory is used for storing temporary files which are not necessary to commit to the repository.
- **`.gitignore`**: This file specifies the files and folders that should be ignored by Git.
- **`LICENSE`**: This file contains the license for the project.
- **`README.md`**: This file contains the documentation for the project, explaining how to set it up and use it.
- **`requirements.txt`**: This file lists the dependencies for the project, making it easier to install all necessary packages.
