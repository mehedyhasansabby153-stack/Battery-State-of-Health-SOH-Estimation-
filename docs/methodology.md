# Methodology

## 1. Dataset

This project uses the NASA Battery Dataset for lithium-ion battery degradation analysis and State of Health (SOH) estimation.

The dataset contains battery cycling measurements recorded under different operating conditions. Charge and discharge cycle data are analyzed to investigate battery degradation behavior.

The raw dataset is not included in this repository.

## 2. Data Preprocessing

The battery cycling data are processed to obtain the relevant measurements required for SOH estimation.

The preprocessing steps include:

* Loading the battery cycling data
* Selecting relevant battery cells and cycles
* Extracting discharge cycle information
* Handling the required data fields
* Organizing the data for subsequent analysis

## 3. SOH Calculation

The State of Health (SOH) of a battery is calculated based on its remaining discharge capacity relative to its initial capacity.

The SOH is expressed as:

$$
SOH(\%) = \frac{Capacity_N}{Capacity_1} \times 100
$$

where:

* $Capacity_N$ represents the capacity at the current cycle.
* $Capacity_1$ represents the initial capacity.

A decrease in SOH indicates battery degradation over successive cycles.

## 4. Feature Extraction

Relevant battery characteristics are extracted from the processed cycling data.

The extracted information may include electrical and thermal characteristics such as:

* Voltage
* Current
* Temperature
* Discharge capacity

These features are used to represent the degradation characteristics of the battery.

## 5. Data Representation

The processed battery measurements are transformed into an appropriate representation for machine learning and deep learning analysis.

The selected representation is used to preserve relationships among battery operating characteristics while making the data suitable for image-based deep learning models.

## 6. Data Augmentation

Data augmentation is investigated to increase the diversity of the training data and improve model generalization.

Synthetic samples are generated using an appropriate generative modeling strategy while maintaining the characteristics of the original battery data.

## 7. Model Development

Machine learning and deep learning models are developed for battery SOH analysis.

The models are trained using the processed battery data and evaluated based on their ability to accurately estimate battery health.

## 8. Training Procedure

The prepared dataset is divided into appropriate subsets for model development and evaluation.

The training process includes:

1. Preparing the input data
2. Defining the model architecture
3. Training the model
4. Monitoring the training process
5. Saving the trained model
6. Evaluating model performance

## 9. Evaluation

The developed models are evaluated using standard regression metrics.

The main evaluation metrics include:

* Mean Absolute Error (MAE)
* Root Mean Square Error (RMSE)
* Coefficient of Determination ($R^2$)

These metrics are used to compare model performance and assess the accuracy of SOH estimation.

## 10. Reproducibility

The project is organized to support reproducible research.

The `notebooks/` directory contains the experimental workflow, while the `src/` directory contains reusable source-code modules.

Dataset information and processing details are documented separately to facilitate reproduction of the experiments.
