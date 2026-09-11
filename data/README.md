# Dataset

## Overview

This project uses the NASA Battery Dataset for lithium-ion battery degradation analysis and State of Health (SOH) estimation.

The dataset contains charge and discharge cycle measurements collected from lithium-ion batteries during different stages of degradation.

## Dataset Source

NASA Ames Prognostics Center of Excellence

The original dataset should be obtained from the official dataset source or the corresponding publicly available repository.

## Data Used in This Study

The dataset is processed to extract relevant battery cycling information required for SOH estimation and subsequent machine learning and deep learning experiments.

The processed data include battery measurements such as:

* Voltage
* Current
* Temperature
* Discharge capacity
* Cycle information

## Data Processing

The raw battery data are processed before being used for model development.

The main processing steps include:

1. Selecting relevant battery cells
2. Extracting discharge cycles
3. Calculating battery SOH
4. Extracting relevant features
5. Preparing the data for model training and evaluation

## Data Availability

The raw dataset is not included in this repository because of dataset size and data management considerations.

Users should obtain the dataset from the original source and place the required files in the appropriate local data directory before running the experiments.

## Directory Structure

```text
data/
└── README.md
```

Raw and processed datasets should not be committed to the repository unless specifically required and permitted.
