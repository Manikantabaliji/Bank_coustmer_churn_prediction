<h1>Bank Coustmer Churn Prediction using CNN</h1>

<p>This repository contains a Python script that uses TensorFlow and Keras to predict bank churn based on a given dataset. The script preprocesses the data, creates a neural network model, trains the model, evaluates its performance, and visualizes the results.</p>

<h2>Dataset</h2>
<p>The dataset 'Bank_churn.csv' contains various features related to bank customers, with the target variable being 'Exited' which indicates whether a customer churned or not.</p> 

<h3>Installs</h3>
pip install pandas tensorflow scikit-learn seaborn matplotlib


## Code Overview

The script follows these main steps:

### 1. Loading and Preprocessing the Dataset:

- Unnecessary columns ('RowNumber', 'CustomerId', 'Surname') are removed.
- Categorical variables like 'Gender' are encoded into numerical values.
- One-hot encoding is applied to the 'Geography' feature.
- Numerical features are scaled using Min-Max scaling.

### 2. Building the Neural Network Model:

- A sequential neural network is constructed using Keras.
- The input layer has 7 neurons with the ReLU activation function.
- A hidden layer with 5 neurons and ReLU activation is added.
- The output layer with 1 neuron uses the sigmoid activation for binary classification.

### 3. Compiling the Model:

- The model is compiled with the Adam optimizer.
- Binary Cross-Entropy is used as the loss function.
- Accuracy is chosen as the evaluation metric.

### 4. Training the Model:

- The model is trained on the training data for 100 epochs.

### 5. Evaluating the Model:

- Model performance is evaluated on the test data.

### 6. Generating a Classification Report:

- A classification report is generated to assess precision, recall, and F1-score.

### 7. Visualizing the Confusion Matrix:

- A confusion matrix is created using TensorFlow's 'tf.math.confusion_matrix'.
- The confusion matrix is visualized using Seaborn's heatmap.

## Results

The script provides insights into the model's performance through the classification report and the visual representation of the confusion matrix. Feel free to explore and adapt the code according to your needs!


