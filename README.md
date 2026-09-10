# Room Occupancy Detection

A machine learning project that predicts whether a room is occupied or unoccupied using environmental sensor readings.

## Overview

Room occupancy can be estimated from changes in environmental conditions such as temperature, humidity, light and CO₂ levels. This project uses these sensor readings to build a classification model that identifies the occupancy status of a room.

## Model

A **Random Forest Classifier** is used to learn the relationship between the sensor readings and occupancy status. The trained model is then used to predict the occupancy of new sensor readings.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Google Colab

## Dataset

This project uses the **UCI Occupancy Detection Dataset**, which contains environmental sensor measurements collected from an office environment.

### Dataset Link

[UCI Occupancy Detection Dataset](https://archive.ics.uci.edu/dataset/357/occupancy-detection)

## Features Used

The model uses five environmental features:

1. Temperature
2. Humidity
3. Light
4. CO₂
5. HumidityRatio

**Target:** `Occupancy`

- `0` → Unoccupied
- `1` → Occupied

## Machine Learning Approach

The project follows these steps:

1. Load the occupancy dataset
2. Separate input features and target values
3. Train a Random Forest classification model
4. Predict occupancy on the test dataset
5. Evaluate the model using accuracy
6. Test the model with a new sensor reading

## Model

**Random Forest Classifier**

```python
RandomForestClassifier(
    n_estimators=100,
    random_state=42
)

## Results

The Random Forest Classifier achieved a **95.35% test accuracy** on the test dataset. The model was also tested with a new set of environmental sensor readings to predict whether the room was occupied or unoccupied.

