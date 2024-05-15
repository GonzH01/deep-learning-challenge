# AlphabetSoupCharity Deep Learning Analysis

## Overview of the Analysis
The purpose of this analysis is to develop and optimize deep learning models using TensorFlow to predict whether charitable organizations will be successful based on various features provided in the dataset.

## Results

### [AlphabetSoupCharity_Optimization1.ipynb](AlphabetSoupCharity_Optimization1.ipynb)
- **Data Preprocessing**:
  - Target Variable: IS_SUCCESSFUL
  - Features: All columns except 'EIN' and 'NAME'
  - Removed Variables: 'EIN' and 'NAME'
- **Model Architecture**:
  - Two hidden layers: 80 neurons in the first layer and 30 neurons in the second layer
  - Activation functions: ReLU for hidden layers, sigmoid for output layer
- **Compiling, Training, and Evaluating the Model**:
  - Training: 100 epochs
  - Achieved Accuracy: 72.73%
- **Steps Taken to Increase Model Performance**: Increased neuron count in hidden layers, reduced epochs.

### AlphabetSoupCharity_Optimization2
- **Data Preprocessing**:
  - Same as Optimization1
- **Model Architecture**:
  - Two hidden layers: 120 neurons in the first layer and 60 neurons in the second layer
  - Activation functions: ReLU for first hidden layer, tanh for second hidden layer, sigmoid for output layer
- **Compiling, Training, and Evaluating the Model**:
  - Training: 50 epochs
  - Achieved Accuracy: 72.42%
- **Steps Taken to Increase Model Performance**: Adjusted activation functions.

### AlphabetSoupCharity_Optimization3
- **Data Preprocessing**:
  - Similar to Optimization1 and Optimization2 with minor changes in cutoff values.
- **Model Architecture**:
  - Two hidden layers: 100 neurons in the first layer and 50 neurons in the second layer
  - Activation functions: ReLU for hidden layers, sigmoid for output layer
- **Compiling, Training, and Evaluating the Model**:
  - Training: 150 epochs
  - Achieved Accuracy: 72.71%
- **Steps Taken to Increase Model Performance**: Adjusted preprocessing parameters.

## Summary
In summary, although the deep learning models developed in this analysis showed promise, they fell short of achieving the 75% accuracy target. Despite numerous optimization efforts, such as tweaking model architecture, activation functions, and preprocessing parameters, the accuracy remained below the mark. One challenge encountered during the optimization process was that by increasing bin count and values per bin resulted in Google Colab crashes due to RAM limitations. Further improvements could be made by experimenting with different architectures, activation functions, and optimization techniques. Additionally, exploring ensemble methods or other machine learning algorithms might provide better performance for this classification problem.
