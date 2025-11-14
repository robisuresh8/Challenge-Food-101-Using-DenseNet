# Food-101 Image Classification using DenseNet

This project is a deep learning experiment to classify images from the **Food-101 dataset** using a **DenseNet** model. The entire workflow, from data preprocessing to model training and evaluation, is contained within the `Challenge_Food_101_Using_DenseNet.ipynb` Jupyter Notebook.

## Project Overview

The goal is to build a model that can accurately identify 101 different types of food, a challenging fine-grained classification task. This implementation uses a DenseNet architecture, a Convolutional Neural Network (CNN) known for its feature reuse and efficiency, implemented in Keras (TensorFlow).

## Technology Stack

* **Python**
* **Jupyter Notebook**
* **TensorFlow** & **Keras** (for model building, training, and data generators)
* **NumPy** (for numerical operations)
* **Matplotlib** (for plotting images and results)
* **scikit-learn** (likely for metrics like classification reports or confusion matrices)

## How to Run This Project

### 1. Clone the Repository

```bash
git clone [https://github.com/robisuresh8/Challenge-Food-101-Using-DenseNet.git](https://github.com/robisuresh8/Challenge-Food-101-Using-DenseNet.git)
cd Challenge-Food-101-Using-DenseNet
```

### 2. Set Up a Python Environment

It is highly recommended to use a virtual environment.

```bash
# Create a virtual environment
python -m venv venv

# Activate it
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies

You will need to install the core libraries for deep learning and data science.

```bash
pip install jupyterlab tensorflow numpy matplotlib scikit-learn
```

### 4. Download the Food-101 Dataset

The Food-101 dataset is very large (~5GB) and is not included in this repository. The notebook will likely download this dataset automatically (e.g., using `tensorflow_datasets`) or it may require you to download it manually from the official source: [https://data.vision.ee.ethz.ch/cvl/food-101/](https://data.vision.ee.ethz.ch/cvl/food-101/)

**Note:** Check the first few cells of the notebook for data loading instructions. You may need to adjust file paths to match where you've saved the dataset.

### 5. Run the Jupyter Notebook

Start Jupyter Lab (or classic Jupyter Notebook) to open the project.

```bash
# To start Jupyter Lab
jupyter lab

# Or to start the classic notebook
jupyter notebook
```

From the browser interface, open `Challenge_Food_101_Using_DenseNet.ipynb` and run the cells sequentially to train the model and see the results.

## About the Model

**DenseNet (Densely Connected Convolutional Networks)** is a state-of-the-art CNN architecture. Its key feature is that each layer is connected to every other layer in a feed-forward fashion. This helps in mitigating the vanishing-gradient problem, strengthening feature propagation, and encouraging feature reuse.
