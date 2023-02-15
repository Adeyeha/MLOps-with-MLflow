## MLOPS with MLflow
This is a sample project that demonstrates how to use MLflow to create an MLOps pipeline for machine learning models. The project includes two options for installation: local and Docker.

### Requirements
- Python 3.x
- Jupyter Notebook
- MLflow
- Docker (optional)
- Nginx (optional)

### Installation
#### Local Installation
Clone the repository and navigate to the directory:
``` sh
git clone https://github.com/Adeyeha/MLOps-with-MLflow.git
cd <repo-directory>
```
Create a virtual environment and activate it:
``` sh
python3 -m venv env
source env/bin/activate
```
Follow Instructions on Notebook `Getting-Started-with-Mlflow.ipynb` in `experiments` directory

#### Docker Installation
Clone the repository and navigate to the directory:
```sh
git clone https://github.com/Adeyeha/MLOps-with-MLflow.git
cd <repo-directory>
```
Run Docker Compose:
```sh
docker-compose build
docker-compose up
```
### How to use
Start the Jupyter Notebook server:
```sh
jupyter notebook
```
Navigate to the notebook `Getting-Started-with-Mlflow.ipynb` and run the cells to train and deploy the machine learning model.

To track the model using MLflow, open a separate terminal window and navigate to the project directory. Then, start the MLflow tracking server:

``` sh
mlflow server --host 0.0.0.0
```

To view the MLflow tracking UI, open a web browser and navigate to http://localhost:5000.

### Contents
The `Getting-Started-with-Mlflow.ipynb` notebook contains the following sections:
- Data preparation: Preprocessing the data and splitting it into training and testing datasets.
- Training the model: Training a machine learning model using scikit-learn and saving the model in MLflow.
- Tracking the model: Starting an MLflow experiment and logging the model parameters, metrics, and artifacts.
- Deploying the model: Deploying the model as a REST API using MLflow.
- Serving the model: Testing the deployed model by sending requests to the API.

### Contributing
If you want to contribute to this project, please create a pull request with a detailed description of your changes.

### Author
[Temitope Adeyeha](https://github.com/Adeyeha)

