# Chicken Disease Classification

This project aims to classify chicken fecal samples into two categories: diseased (Coccidiosis) and healthy. The classification is based on analyzing images of the fecal samples using computer vision techniques.


## Project Structure

The project follows a modular structure, consisting of several stages and pipelines which includes :-

1. `stage_01_data_ingestion.py`: This stage is responsible for data ingestion. It includes functions for downloading, extracting, and preprocessing the dataset.
2. `stage_02_prepare_base_model.py`: In this stage, the base model for the classification task is prepared. It involves loading a pre-trained model, modifying it if necessary, and preparing it for training.
3. `stage_03_training.py`: The training stage is responsible for training the model using the prepared dataset. It includes functions for data augmentation, model training, and saving the trained model.
4. `stage_04_evaluation.py`: This stage focuses on evaluating the performance of the trained model. It includes functions for loading the trained model, performing inference on test data, and calculating evaluation metrics.

## Requirements

To run this project, you need the following requirements:

- Python (version 3.8 or above)
- TensorFlow 
- Flask 
- DVC 

Make sure you have installed the required dependencies before running the project.

## Workflows

1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml


## Usage

1. Clone the repository:

```bash
git clone https://github.com/Pratik94229/Chicken-Disease-Classification-Project

```
```
cd Chicken-Disease-Classification-Project
```

2. Create a conda environment after opening the repository
```
conda create -p venv python==3.8 
conda activate venv/

```
3. Install the dependencies:

```bash
pip install -r requirements.txt
```


4. Finally run the following command

```
python app.py

```

5. Open Terminal

### DVC cmd
```
dvc init
dvc repro

```
6. For visualizing pipeline
```
dvc dag

```

7. Flask App:

To create a front-end interface for the application, run the Flask app:

```bash
python app.py
```

8. Access the app:

Open your browser and go to 

localhost to access the application.

# Conclusion
In summary, this project showcases the effective classification of chicken fecal samples into two categories: diseased or healthy, employing advanced computer vision methodologies. Its organized, modular structure, coupled with the utilization of pipelines, ensures that the workflow is not only comprehensible but also readily replicable. Furthermore, the incorporation of a Flask application empowers users to effortlessly engage with the classification model.
