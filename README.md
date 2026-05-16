# Breast Cancer Diagnosis Using MLP



## Project Description



This project is a medical diagnosis classification project using the Breast Cancer dataset.



The main goal of the project is to build a Multilayer Perceptron (MLP) neural network that can classify breast cancer tumors as either benign or malignant based on numerical medical features.



This project was implemented using Python, PyTorch, Scikit-learn, Pandas, and Matplotlib.



---



## Problem Type



This is a binary classification problem.



The model predicts one of two classes:



- Malignant

- Benign



---



## Dataset



The dataset used in this project is the Breast Cancer Wisconsin dataset from Scikit-learn.



Dataset source:



https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load\_breast\_cancer.html



The dataset contains:



- 569 samples

- 30 numerical features

- 2 target classes: malignant and benign



Each sample contains medical measurements related to cell nuclei, and the target represents whether the tumor is malignant or benign.



---



## Project Steps



The project follows these main steps:



1. Import required libraries

2. Load the Breast Cancer dataset

3. Split the data into training, validation, and testing sets

4. Apply StandardScaler for feature scaling

5. Convert the data into PyTorch tensors

6. Build an MLP neural network model

7. Train the model using the training data

8. Validate the model using validation data

9. Plot training and validation loss curves

10. Plot training and validation accuracy curves

11. Evaluate the final model on test data

12. Conduct two experiments with different parameters

13. Compare the results



---



## Data Preprocessing



The dataset was preprocessed using the following steps:



- Checked and loaded the numerical features

- Split the dataset into training, validation, and testing sets

- Applied StandardScaler to normalize the feature values

- Converted the data into PyTorch tensors



Feature scaling was important because the dataset contains numerical values with different ranges.



---



## Model Architecture



The implemented model is a Multilayer Perceptron (MLP).



The model includes:



- Input layer

- Hidden layers

- Activation functions

- Output layer



Since this is a binary classification problem, the output layer uses the Sigmoid activation function.



---



## Experiment 1



Experiment 1 used the following settings:



| Parameter | Value |

|---|---|

| Activation Function | ReLU |

| Hidden Neurons | 32, 16 |

| Learning Rate | 0.01 |

| Optimizer | Adam |

| Loss Function | BCELoss |



---



## Experiment 2



Experiment 2 used the following settings:



| Parameter | Value |

|---|---|

| Activation Function | Tanh |

| Hidden Neurons | 64, 32 |

| Learning Rate | 0.001 |

| Optimizer | Adam |

| Loss Function | BCELoss |



---



\## Results Comparison



| Experiment | Activation Function | Hidden Neurons | Learning Rate | Final Test Loss | Test Accuracy |

|---|---|---|---|---|---|

| Experiment 1 | ReLU | 32, 16 | 0.010 | 0.180581 | 0.964912 |

| Experiment 2 | Tanh | 64, 32 | 0.001 | 0.064225 | 0.982456 |



---



\## Best Experiment



Experiment 2 achieved the best performance.



It achieved:


- Final Test Loss: 0.064225

- Test Accuracy: 0.982456



This means that Experiment 2 achieved approximately 98.25% test accuracy.



Experiment 2 performed better than Experiment 1 because it achieved higher accuracy and lower loss. The smaller learning rate helped the training process become more stable, and the larger number of neurons gave the model more ability to learn patterns from the dataset.



However, this does not mean that Tanh is always better than ReLU. In this specific experiment, Tanh with more neurons and a smaller learning rate achieved better results.



---


## Visualizations



The project includes the following visualizations:



- Training vs Validation Loss curve

- Training vs Validation Accuracy curve

- Validation Loss comparison between experiments

- Validation Accuracy comparison between experiments



These plots help show how the model learned during training and how the experiments performed differently.



---



## How to Run the Project


### 1. Clone the repository



```bash


