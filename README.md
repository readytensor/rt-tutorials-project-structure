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
│   ├── errors/
│   ├── hpt_outputs/
│   └── predictions/
├── src/
│   ├── config/
│   ├── data_models/
│   ├── hyperparameter_tuning/
│   ├── prediction/
│   ├── preprocessing/
│   ├── schema/
│   └── xai/
├── tests/
│   ├── integration_tests/
│   ├── performance_tests/
│   └── unit_tests/
│       ├── <mirrors /src structure>
│       └── ...
├── tmp/
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

- **`/examples`**: This directory contains all files you want to use as examples. Typically, these would be small data files that can be used as examples for the ML project.
- **`/examples`**: This directory contains all files you want to use as examples. Typically, these would be small data files that can be used as examples for the ML project.
- **`/inputs`**: This directory contains all the input files for your project, including the data and schema files. The data is further divided into testing and training subsets.
- **`/model/artifacts`**: This directory is used to store the model artifacts, such as trained models and their parameters.
- **`/outputs`**: The outputs directory contains sub-directories for error logs, and hyperparameter tuning outputs, and prediction results. Note that model artifacts should not be saved in this directory. Instead, they should be saved in the `/model/artifacts` directory.
- **`/src`**: This directory holds the source code for the project. It is further divided into various subdirectories such as `config` for configuration files, `data_models` for data models for input validation, `hyperparameter_tuning` for hyperparameter-tuning (HPT) related files, `prediction` for prediction model scripts, `preprocessing` for data preprocessing scripts, `schema` for schema scripts, and `xai` for explainable AI scripts.
- **`/tests`**: This directory contains all the tests for the project. It contains sub-directories for specific types of tests such as unit tests, integration tests, and performance tests. For unit tests, the directory structure should mirror the `/src` directory structure. For example, if you have a `preprocessing` folder in the `/src` directory, then tests corresponding to the scripts under `src/preprocessing` should be placed in the `/tests/unit_tests/preprocessing` directory.
- **`/tmp`**: This directory is used for storing temporary files which are not necessary to commit to the repository.
- **`.gitignore`**: This file specifies the files and folders that should be ignored by Git.
- **`LICENSE`**: This file contains an MIT license for the project. You can change this to any other license you want.
- **`README.md`**: This file contains the documentation for the project, explaining how to set it up and use it.
- **`requirements.txt`**: This file lists the dependencies for the project, making it easier to install all necessary packages.
